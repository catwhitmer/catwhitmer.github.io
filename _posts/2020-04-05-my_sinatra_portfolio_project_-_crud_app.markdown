---
layout: post
title:      "My Sinatra Portfolio Project - CRUD App"
date:       2020-04-06 02:42:47 +0000
permalink:  my_sinatra_portfolio_project_-_crud_app
---


  For the Sinatra CRUD App Project I decided to create an app that allows users to be a part of a gaming library where they can see a list of popular games. My whole life I have been a gamer  and I enjoy reading which kinds of games other people recommend. I am always on the lookout for the next game to play.

Getting started
 For the first step I needed to decide what I wanted the app to do and how it should be structured. Users need to be able to sign up, log in, create game entries, see all the games and edit and delete their games. To create the structure I decided on two models; a game and a user. For the attributes each game should have a name, genre and foreign key (determined later through associations). The user gets the attributes of name, email and password. Then it was time to determine the associations: a user has many games and the game belongs to the user. Since the games belong to the user it needs a foreign key. 

Setting up the DB
 Next came adding the database so that there was data to work with. Setting up the migrations for the model tables was easy enough. I also created some seeded data, added the models, and made sure I had everything set up for coding out the routes.

Coding the routes
  The thought process was to go in order of the user by first creating the sign up and log in routes, double checking that they worked before moving on. Coding the routes was fun but it was easy to make mistakes so it required constant double checking. At one point the entire app stopped working. It turned out that my “user” was logged in permanently. It took some time to figure out that one little typo could do so much damage. I definitely learned to check all my code from now on. 

Adding some style
  The last thing I wanted to do is add some style to the app. I didn't want it to look too generic. I pretty much worked route by route on the style, trying to create a basic uniformed structure. Spending a lot of time on CSS was something I avoided because I felt that the function of the app was more important.

What I learned
* Make sure to reread all of your code. I wasted a whole day due to a spelling error that I missed in a place I didn’t bother to look.
* Ask for help! A second pair of eyes might spot a mistake you made
* This project was a lot of fun to create. I learned a lot!!!


