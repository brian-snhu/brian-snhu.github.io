# Brian Russell - ePortfolio

## Refinement Plan & Code Review

### Introduction
<p align="left">
  The refinement plans and code review are for an active online game that I am the current head programmer, developer, and server owner of Free Infantry Online. The software project of question is the game's login screen and launcher. Currently, a user has to ask in our Discord chat, or website for credential retrievals. To mitigate this, the refinement plan is to add a forgot username and password button that will provide credentials either to the users email, or to the launcher screen itself.
</p>

### Software Engineering & Design
<p align="left">
  For the software design aspect, I decided to have the forgot password button use its own Windows form. This will provide less clutter on the Main form as well as its own partial class that can hold all button events needed. Once the forgot password button is clicked, it will raise an event handler that will create and open a new recovery form with clickable buttons. In the recovery form, there will be two buttons that ask the user if they are recovering a username or a password. Then, there will be an an OK or Cancel button for submission or cancelization.
</p>

### Algorithms and Data Structures
<p align="left">
  In algorithms and data structures, I have will be expanding the AccountController class handler. The handler will be used to send the recovery request to the server in an asyncronous method. I plan on using JSON to serialize and deserialize any data to and from the server as well as HTTP status codes that will be used to give visual messages of what is actually happening. These messages will give a brief but straight to the point message that will tell the user of any potential errors that may have happened during the recovery process.
</p>

### Databases
<p align="left">
  For Databases, the refinement plan is to have the server deserialize the data in JSON format. This will give me the requested data and input that as an object to be validated by the server. The server will do checks for data corruption, null data, matching tokens that were generated previously by the server, and the users credentials against the database table. Also, the database will be expanded to include a new database table that has the reset token information, user identification, their associated account for email, username, and password retrieval, as well as a boolean that will check if the reset token was used or not. Each function will be handled within the proper HTTP GET, PUT, or POST methods.
</p>

### Code Review
<div align="center">
  <iframe width="560" height="315" src="https://www.youtube.com/embed/P-7gncW4qCk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

**Portfolio Links**<br>
* [Professional Self-Assessment](https://brian-snhu.github.io/)<br>
* [Enhancement One](https://brian-snhu.github.io/enhancementone.html)<br>
* [Enhancement Two](https://brian-snhu.github.io/enhancementtwo.html)<br>
* [Enhancement Three](https://brian-snhu.github.io/enhancementthree.html)

**Project Links**<br>
* [Infantry Launcher](https://github.com/brian-snhu/Infantry-Launcher)<br>
* [Mini Account Server](https://github.com/brian-snhu/Infantry-MiniAccountServer)
