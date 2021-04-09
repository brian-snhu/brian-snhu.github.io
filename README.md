## Brian Russell's ePortfolio for CS-499

Self-Assessment Here

## Code Review
<p align="left">
    The project in question is a current online game called Free Infantry Online, a defunct Harmless Games/Sony game. A group of dedicated software developers (including myself) decided to continue their legacy with Sony's expressed permission. For this game written in C#.Net, I decided to create a new launcher that will allow a person to log into the game. The launcher is designed and programmed by me with graphics provided be another team member. Its function is to allow a user to connect to the account server and verify their credentials before given access to the game.
</p>

## Enhancement One: Software Engineering & Design
<p align="left">
    In this category, the plan was to allow the software to have a one way communication line between the call functions and the forms. The return data would be event calls that gave the required responses only. I modified the forgot password button to have its own Windows Form. The functionality is to provide the user with a window that has a username and a password button which will decide what the request is. After the user picks, it will send this data using JSON to the server and wait for a response. Once returned, it will tell the user their username or tell them to check their email for a password reset.
</p>

https://github.com/brian-snhu/Infantry-Launcher/commit/78d97cd357501f6a1c78462b511afc1bf763e9ef

## Enhancement Two: Algorithms and Data Structure
<p align="left">
    For Algorithms and Data Structures, the enhancement plan was to add the necessary coding for the recovery request to be sent to the account server. In order to do so, a new class called IStatus will be constructed. This class will hold all the public objects and enumerators for requests and responses. Each request and response will be serialized and deserialized using JSON. Also, to reflect the changes, all data handlers will be changed to reflect the IStatus class.  
</p>

https://github.com/brian-snhu/Infantry-Launcher/commit/71f93f09befaf5d65e4a620477ee7d875653ea86

## Enhancement Three: Databases
<p align="left">
    In the Database enhancement plan, the initial request for recovery was added. In order to properly deconstruct the JSON object, a data table in MSSQL will be made that has the users account information, username, token, expire date, and a true or false boolean to validate if the token was used or not. Then, the listener handler will have the validation functions that check for any corrupted or unwanted data that is sent to it. Once the validation is completed and meets the requirements, an email is sent to the user that was registered with the account with either a password reset token link or their username. If it is a password reset token, then the email will trigger a password reset response from the account server that will allow the user to change theirs.
</p>


**Project Links**<br>
* [Infantry Launcher](https://github.com/brian-snhu/Infantry-Launcher)<br>
