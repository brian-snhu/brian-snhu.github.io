# Brian Russell - ePortfolio

## Enhancement Three: Databases
### The Artifact
<p align="left">
  In this artifact, it is the game server’s account management server. This server controls who has access to the game by data being sent from the launcher. The user’s credentials are verified by this server and if successful, the game client will launch with a session ID provided by this server to the player’s login object. This server was created in 2018 initially and upgraded over time since then.
</p>

### Inclusion
<p align="left">
    The artifact reflects the JSON work that I introduced to the game server. Many software developers use some type of account recovery system that can retrieve or change a user's account credentials. This idea was introduced a while ago, but it was never implemented until now. The use of JSON conversions and how the data can interact with the database has potential to show companies how I can manipulate data. Specifically, how a request for a password change turns into a generated clickable link that is emailed to the user. Because the server never had this ability, the artifact was improved by adding this.
</p>

### Enhancement Objective
<p align="left">
    The enhancement objective has been achieved because the use of JSON conversions was the intended idea. I have added the Recover Request Model and the Reset Request Model classes in reflection format of the launcher data it is receiving. Also, I have added another if statement in the POST for recovery that now takes the object and deserializes it, then checks for any manipulated data. Within the HTTP handler, the data is checked for either a username or password recovery request. If the data is a username recovery, then it will send this data to the database client that will check the parameters within the database tables. If successful, it returns true and the username, otherwise false. Once true, the function sends an email which took a bit to debug and get the format right. I had to create an email account just for these reset requests. As for the password recovery portion, it is passed to the database client to create an MD5 hash token that is generated into an SHA1 reversed 8bit format and sent to the user's email. Once the user clicks the link, it continues back to the account server to be verified that this was generated and if successful, the user is given a request to change their password on the launcher.
</p>

### Reflection
<p align="left">
    The use of JSON for HTTP requests and responses can give a program an easier way to communicate to another server or program. What I learned is that the web request must be formatted correctly, otherwise an error message will be thrown, or no response at all. Using Visual Studio’s debugging tool, this method made quick work with the errors I was generating. Also, the database side took a while to query and modify the SQL tables correctly. I had to do it in a specific sequence, so the data was not corrupted.
</p>

**Portfolio Links**<br>
* [Professional Self-Assessment](https://brian-snhu.github.io/)<br>
* [Refinement Plan & Code Review](https://brian-snhu.github.io/codereview.html)<br>
* [Enhancement One](https://brian-snhu.github.io/enhancementone.html)<br>
* [Enhancement Two](https://brian-snhu.github.io/enhancementtwo.html)

**Project Links**<br>
* [Infantry Launcher](https://github.com/brian-snhu/Infantry-Launcher)<br>
* [Mini Account Server](https://github.com/brian-snhu/Infantry-MiniAccountServer)
