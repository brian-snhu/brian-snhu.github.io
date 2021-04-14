# Brian Russell - ePortfolio

## Enhancement One: Software Engineering & Design
### The Artifact
<p align="left">
    The artifact for my ePortfolio in question is a game launcher designed for the free online game called Free Infantry Online. The software is designed to be a login point for any user. It takes a username and a password to access the game engine which is in a separate game program. This login program contacts the account server with the provided credentials and if correct, allows you to play the game. If unsuccessful, it lets you know with a brief detailed error message. This was created in February of 2020 and repolished in September of 2020.
</p>

### Inclusion
<p align="left">
    One of the reasons of this artifact to be presented in my portfolio is it allows people to see how my software design elements, procedures, and readability is utilized. Instead of having one file cluttered with all functions needed, I like to have separate functions specified in different files with access points or data manipulation without full access to the system. For example, instead of having a Windows form access another Windows form within it, it calls another form that is outside of the main form. In other words, the main form file calls the sub form file, and all functionality for this new form is in this sub form file. This was one improvement that I added while another was the event call for the button that accesses this new form called the Recovery Form.
</p>

### Enhancement Objective
<p align="left">
    I believe this is my best work because I was able to design and implement what I wanted it to do from start to finish. The enhancement was met by incorporating the newly created recovery form using Windows Forms. The event callbacks were added into this recovery form to provide information to the user once the process is initiated. For the functionality of the forgot password button, this recovery form and process is invoked by the main form. Although the user does not know what is happening behind the scene, visually, there are error messages for any problems or server errors that could occur.
</p>

### Software Design and Engineering: Reflection
<p align="left">
    Since I am familiar with C# .Net, the process of design to implementation was quick. The design feature will add an easier way for players to recover their accounts without relying on a server administrator to complete their request. The use of debugging was a big help when I first started this project. Without debugging, I would have not found JSON errors with serialization and deserialization. One thing I did learn during this project is that readability is key in the design. I am not a person that likes programming clutter as I call it. I like to be able to see and follow the process of each function.
lose the window.
</p>

**Portfolio Links**<br>
* [Professional Self-Assessment](https://brian-snhu.github.io/)<br>
* [Refinement Plan & Code Review](https://brian-snhu.github.io/codereview.html)<br>
* [Enhancement Two](https://brian-snhu.github.io/enhancementtwo.html)<br>
* [Enhancement Three](https://brian-snhu.github.io/enhancementthree.html)
