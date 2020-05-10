---
layout: post
title:      "My Rails Project"
date:       2020-05-10 23:23:47 +0000
permalink:  my_rails_project
---


First, I cannot believe this project is complete. I thoroughly enjoyed it and it really taught me how everything fits together. 

For the third project I created an app that gives a user the ability to make appointments for different types of massages. The user is also able to create custom massages and then make appointments for them. My app consists of three models:

* User: has many massages and many appointments through massages
* Appointment: belongs to the user and the massage
* Massage: has many users and many appointments through the user

After the model's relationships were set up, I created my migrations and database.  I thought I had my schema figured out, but I kept having to rollback because of not thinking things through. It took a few tries to figure it out, but it taught me to thoroughly map out my associations and attributes before coding anything at all. After that I worked systematically by first making sure a user can sign up and log in. Then I focused on one model at a time, leaving the join model for last. The nested routes were a bit tricky, but watching a few videos on learn instruct really helped to figure out how to properly set those up. Looking back, I wish I would have nested the appointments under the user and not the massages, but I might change that eventually.

The last tasks I focused on were adding omniauth, styling the pages, and adding helper methods to assist with authentication. I honestly struggled more with the styling than with omniauth. The guides learn.co gives you are very easy to follow: https://learn.co/tracks/online-software-engineering-structured/rails/auth/omniauth 
However, styling was a lot of trial and error. I ended up using the gem bootstrap. The website getbootstrap had some great simple information on styling your pages. 

What I learned
* Take the time to thoroughly map out your schema
* Spend some time on how to style your app
* Check for spelling errors

