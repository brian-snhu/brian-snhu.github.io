# Brian Russell - ePortfolio

## Enhancement Two: Algorithm & Data Structures
### The Artifact
<p align="left">
    The artifact is a continuation of the game launcher for Free Infantry Online as previously mentioned. For the algorithm and data structure portion, the recovery request for the game launcher is forwarding the request to the appropriate handler which is the AccountServer class. This class will serialize the data that the user inputted and send it out using JSON and HTTP. For its return values, I have a switch case scenario that will look for the return status codes and either say OK and give a true value or false and give an error message. The data structure itself uses a recovery request object that has two string values and a Boolean value within its object class. To simplify the return data, an IStatus class was created. The IStatus class and its enumerators are used to figure out what the server return code is and possibly any error message sent with or a 200 OK status code. Also, all handlers have been updated to reflect the IStatus class changes.
</p>

### Inclusion
<p align="left">
    The chosen artifact gives a brief look into my thought process from start to finish. I value having things visually appealing at home and in a business setting which is shown in my work as well. For this artifact, it shows how creative I can be and my knowledge of the C# .Net language. To give an example, within the programming itself, I use data structured objects and classes to obtain the needed information then parse it into a readable string that the user can read. One can see this in the AccountServer class where I am using a switch statement that first calls the AccountServer.RecoverAccount function, then awaits the return data. Once the data is retrieved, it sets a string variable and opens a message box with that string for the user to visually see what happened.
</p>

### Enhancement Objective
<p align="left">
    The enhancement objective was to have the data sent out and returned in an error free manner. What I did was set a data structure for the recovery request object and then have it forwarded to another function that will send it to the game server. Once the server does its checks and sends back an HTTP request response, I parse this data using the IStatus class and its enumerators into a readable string. Also, I have added some data checks within the server to verify the data that is being sent by the game launcher. This is the enhancement objective.
</p>

### Reflection
<p align="left">
    With Windows being the main library source of C#.Net and using Visual Studio in conjunction with it, the debugging process as well as the code writing process made it easier. Although this is not the case with other languages, I find that Visual Studio offers a lot more than other debuggers. I used a local server to verify the data that was being sent to the server. Then, I adjusted some of the variables that were giving misinterpreted data. What I learned is debugging is an important step in the software development process just as much as completing the task is.
</p>

**Portfolio Links**<br>
* [Professional Self-Assessment](https://brian-snhu.github.io/)<br>
* [Refinement Plan & Code Review](https://brian-snhu.github.io/codereview.html)<br>
* [Enhancement One](https://brian-snhu.github.io/enhancementone.html)<br>
* [Enhancement Three](https://brian-snhu.github.io/enhancementthree.html)

**Project Links**<br>
* [Infantry Launcher](https://github.com/brian-snhu/Infantry-Launcher)<br>
* [Mini Account Server](https://github.com/brian-snhu/Infantry-MiniAccountServer)
