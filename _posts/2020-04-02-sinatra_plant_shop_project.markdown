---
layout: post
title:      "Sinatra Plant Shop Project"
date:       2020-04-02 04:45:32 -0400
permalink:  sinatra_plant_shop_project
---


This section of the curriculum really brings several concepts together.  Founded still in object oriented programming to a degree, it's the culmination of many lessons, and shows how different schools of thought can seamlessly work together to create a webpage that allows for users to create, save, and edit objects that persist in a database.

The process of creating this project really starts with the organization of the entire thing, which comes down to routes.  It's helpful to visually which pages will link to which routes, and how those all interact.  Before writing any code, it's a given that one must decide which classes and models to work with.  With this project I chose users and plants.  Users can have many plants, and a plant belongs to a user.  Using active record, it's important to set these associations before anything else.  Then, run rake db:migrate, and if you wish to seed the database as well, rake db:seed.  

There was lots of testing of get and post requests to find the best way to navigate without making redundant routes.  Once one route works, it's easy to run shotgun or rackup config.ru to see the page that it links to.  The challenge with routes mostly comes down to making sure you choose to redirect to a different route in the controller or render a page with erb.  Usually you only want one route per page of erb, so additional routes that need to link to the erb, should redirect to the one rendering it.  I learned you should be somewhat careful with this, especially when you have dynamic routes. 

Dynamic routes are a challenge of their own.  It's good to have the url be specific to what you're looking at without showing uncessary information.  Sometimes just an id is important, other times you want a username and id, depending on what you need to render.  The most common way to form the routes is just to put the variable in the route with brackets and on the other end, the route just needs to include a variable such as '/new/:route', where route is whatever the variable following the redirect after '/new' would be.

When creating erb files, it's mostly basic html, with some embedded ruby.  This part shouldn't take too long, and focusing on creating the perfect web page without any css is hardly the main idea.  Once the page displays everything you need it to display, the form should have a method to route back to whatever page you need to render next after the user submits information. 
