---
layout: post
title:      "Sinatra Portfolio Project - Food Journal"
date:       2020-05-21 05:26:31 +0000
permalink:  sinatra_portfolio_project_-_food_journal
---


I just recently finished my Sinatra Portfolio Project and enjoyed it very much.  Much like the individual CLI project, the Sinatra project was surely a challenge but also quite fun at the same time. 

Surprisingly, at least to me, one of the hardest tasks right out of the gate on this project was coming up with a project idea that met the requirements and also provided a useful function or task.  I approached the project by brainstorming and trying to be cognizant of times in my daily life where I had questions or ideas about something I wanted more information on in my life.  For a few days I kept a little notepad with me which I used to make a list of ideas and concepts.  Ultimately, I decided to try and make a simple application that would help me track my meals and the food I ate.  I named my project the Food Journal.  

To start, I set my project up with two models, a User class and a Meal class.  I had a thought to expand my project to include a third class for Exercise so that this application could also track activity and calories burned in addition to the food and calories consumed.  But for now, I decided to keep the project simple and just focus on food.  Maybe I will circle back to this project in the future and add the Exercise class to capture that component of the process.   

My User class is set up with a "username", "email", and a "password".  A user will only be able to operate the CRUD actions on their own meal journal.  They will not be able to view or edit other user's journals.  I was thinking this area could be another future opportunity to expand the application.  It could be fun and useful for users to have the ability to share, or make public certain aspects of their journals to other users so people can share, comment, and support each other in making healthy food choices together.  

My Meal class is set up with a "name", "date", "calories", "prepared_by", "rating" and "description".  I wanted to have a few different data points tied to each instance of a meal with the idea that down the road the application could be expanded to provide some trends, suggestions, and records that might help a user make more informed decisions about their food intake.  After all, knowledge is power that can be turned into action.  

The application is pretty straight forward.  A User "has many" meals and a Meal belongs to a User.  With this setup I added the foreign key to the Meals table so the relationships could be created appropriately using Active Record.   

Once I got the application up and running and the basic controller actions working correctly I shifted my focus to data validation and handling error messages.  I chose to validate the data from the User and Meal forms within the controllers themselves and to use flash messages to alert the user when an error had occurred.  I found it easiest to place all the flash messages in the View/layout.erb file, rather than within each individual View file.  
![](https://drive.google.com/open?id=1xsr9XPN87tZTpvgv_bqK2d1wR5t8oFFC://)

The result was a displayed error message like the example below in red text:
![](https://drive.google.com/open?id=1QOngI3ll3Xl2NvUzkP2YlSdLE82TXYOq)

I've only completed two of the portfolio projects, so far.  But I have had a similar feeling after finishing them both, a greater sense of clarity.  For both projects I'm finding it quite helpful to put all the lessons and labs together into a kind of final product that is produced from scratch.  It helps me solidify what I have learned and to see how it could be applied in a more real life situation.  This is especially true of this Sinatra project, because it's a web based, database application that's easy to imagine being used in real life. 

I look forward to learning more!









