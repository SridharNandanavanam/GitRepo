README - GitHub Connector (Java)

Overview:
----------
This program demonstrates how to connect to the GitHub REST API using Java
and retrieve data such as repositories for a given user.

Files:
------
- GitHubConnector.java : Main Java file that makes an HTTP GET request to GitHub API.

Requirements:
-------------
- Java 11 or later (for HttpURLConnection support).
- Internet connection.
- (Optional) GitHub Personal Access Token if you want to access private repos
  or increase API rate limits.

Setup:
------
1. Compile the Java file:
   javac GitHubConnector.java

2. Run the program:
   java GitHubConnector

3. By default, the program fetches repositories for the user "octocat".
   You can change the username in the source code:
   String user = "octocat";

Authentication (Optional):
--------------------------
- To access private repositories or avoid rate limits, generate a Personal Access Token
  from GitHub (Settings → Developer Settings → Personal Access Tokens).
- Add the token in the code:
  con.setRequestProperty("Authorization", "token YOUR_TOKEN");

Customization:
--------------
- Change the API endpoint to fetch
