Journal
=======
This here's a small project based on the following link: 'https://learn.microsoft.com/sv-se/aspnet/core/tutorials/first-web-api?view=aspnetcore-8.0&WT.mc_id=dotnet-35129-website&tabs=visual-studio'. I'll be documenting my process to creating the ASP.NET API described in the tutorial.

2024-02-12
-----------
As a short starter, I set up the project and Git repository. I'll continue with the project tomorrow.

2024-02-13
-----------
As usual, my first order of business was clear: deactivate swagger. It's not that I don't see the tool as useful, I just prefer Postman. So I tinkered a little with 'launchSettings.json' and 'Program.cs', and now it works the way I want it.

I'm following the tutorial, as I mentioned above, but I'm also changing a few things somewhat. The tutorial expects the database context class to be placed in the models folder, which I haven't done previously, so I placed it in a new 'Data' folder instead. I'll try not to ignore instructions like this too often - it may come back to haunt me later.

Also I did not expect the scaffold item to generate a full-on controller class for the API. So that caught me off guard.

I've now tested all the HTTP methods, so I've uset Get, Get({"id"}), Post, Put, and Delete. Nothing new; I've done this before. I'm actually pretty sure I've completed this exact tutorial before as well, but not completely certain. Good practice to redo it though, I think. As stated previously, I did completed these tests with Postman. Next up is to prevent over-posting.

2024-02-14
-----------
The rest of the project went well, I ran into no issues. Creating the DTO model and implementing it was new territory for me, so it was a little less obvious to me compared to the other things in the tutorial. So, the project as a whole meant setting up a small API using an in-memory database that handles various HTTP methods to retrieve and send data to the database. The DTO model was for securing a 'secret' string that only authenticated users are to be able to access, unless I am mistaken.