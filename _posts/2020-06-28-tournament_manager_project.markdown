---
layout: post
title:      "Tournament Manager Project"
date:       2020-06-28 16:19:16 -0400
permalink:  tournament_manager_project
---


Written in Ruby on Rails, this project brings together nearly all that we've studied throughout the course up to this date.  This was the toughest, most challenging, or at least largest project involving the most amount of written code I've ever done.  I wrote over 15 views, 5 controllers with methods, and many routes, models, and migrations.  Most of it was by hand, with only slight help from generations, or partials.  

The first step to creating something of this scale is planning.  It's important to come up with models to represent all the data and how they interact.  

You can generate only certain things with rails g, such as migrations, and empty controllers and models.  Beyond that everything must be written by hand.  I opted to generate the models and database migrations for the most part, even though I ended up changing several parts of both after they were made. 

The models need to work together and be one of the last things that you can consider changing in your planning phase.  After the models are set, the whole project is set, because everything is based on how the models relate to each other. 

Despite all of the thing described above, views and controllers alone far outweight all of the other code in the entire project.  Views must contain the display of the entire project, and controllers basically tell them what to do at every turn.  There is some surface level logic in the views, such as controlling what a user sees when at a specific url under conditions that aren't worth of route level changes.   Controllers will generally contain all the logic that has to do with navigation, but in an ideal world, they would be helped by methods in models to control the gathering of data.  
