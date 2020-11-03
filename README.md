# Java_Web_API
November 2020

This back-end web API runs a Wildfly server.  This is how the web API runs.  When the user goes to Postman, and simulates a front-end web call, the user receives a result in JSON.  Almost no HTML was written.

This is a non-enterprise level banking web-API, written in Java.  The following functions are implemented: transfer funds, login, logout, deposit, withdraw, find account given user, find user given account, find accounts by status, create a link between user and account, create user, etc.

After you click on the src (source) folder, then after you click on the main/java/com folder, you'll come to four folders.  Click on DAOUtilities to see utlitity functions common to every function in the dao (data access object) and/or servlets folders.  The Model folder contains classes that get used everywhere else.  

The dao folder contains interfaces and their implementations.  This includes simple SQL scripts that, in production, would be in stored procedures.  It calls the database and returns informaton to the servlet layer.

The Servlet folder is the interface between Postman and the DAO.  It decides if the user has security to perform the operation, executes the desired function, then returns the information back to the caller (Postman, in this case).

Technologies used: Java, SQL, PostresQL, Eclipse

Screenshots:

![Code](https://github.com/MarioThompson0010/Java_Web_API/blob/master/Assets/JavaCode.PNG)
![Result](https://github.com/MarioThompson0010/Java_Web_API/blob/master/Assets/ResultSuccessful.PNG)

