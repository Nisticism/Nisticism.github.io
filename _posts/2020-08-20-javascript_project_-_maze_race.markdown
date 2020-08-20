---
layout: post
title:      "Javascript Project - Maze Race"
date:       2020-08-20 20:59:46 +0000
permalink:  javascript_project_-_maze_race
---


The Javascript module has lead to it's conclusion required the production of one final project.  For this project and the technologies involved it has felt like a culmination of everything I've learned so far.  

To begin, as is often useful while completing large projects, I planned most of the project before programming anything and when I started, I started with the back end.  Creating resources is the first step, for which I decided on mazes, users, and scores.  The choice was between that and adding games in, to have many mazes.  I ended up implementing games in the front end only.

I learned about json serializers to present the data, and created 3 serializer classes for all of the resources.  I handled resource creation with the controllers and routes, and added in another route to find or create users.  

The front end was the most fun.  Creating the entire game's loop and design was something I accomplished after lots of research on html5's canvas, and something called a requestAnimationFrame function, which could run code every frame.  The images and game objects were updated as controlled by the user, and scores could be saved by creating fetch requests to the backend api, with the maze id, user id, and time.  The timer function was also another task that required some research but with such helpful functions such as "setInterval" and "clearInterval" it was not too difficult.  

In the end, the levels were stored as strings in the database.  While initially I wanted a generator, it would be more practical to make levels ahead of time, and have users compete on time.  A maze generator would need to be perfected so users would never get stuck by misplaced blocks, and requires an algorithm that would most likely produce sub-par mazes even though it's still something I'm greatly interested in.  One day I hope this app becomes hosted on a server somewhere, and I can improve it over time.  Overall this game was a good learning experience and the first major javascript project I've completed, and hopefully it's not the end of the story for Maze Race.  
