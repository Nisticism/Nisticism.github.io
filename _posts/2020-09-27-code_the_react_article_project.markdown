---
layout: post
title:      "Code the React Article Project"
date:       2020-09-27 02:24:53 -0400
permalink:  code_the_react_article_project
---

This final project was the culmination of everything I've learned up to this point with Flatiron.  It began in the planning phase where I would be integrating a Rails API.  Aided by endless videos, I set up my models, validations, database, serializers, and the rest of my backend without too much trouble.  I kept in mind that "Likes" were a stretch goal that I eventually wanted to add to "Comments" and "Articles".  Either way, the user had to be able to log in, and create the other models.

The prior lessons prepared me for the formerly foreign landscape of Redux.  Redux seemed to me at first like a rube goldberg machine (and I credit this description to another blog), and never really lost that impression for me - however if built properly, rube goldberg machines can be beautiful, and accomplish tasks that might have multiple components or out of reach goals.  Once I learned redux, I respected the technology for what it could do.  With Redux, I was able to make objects appear and disappear instantly on the page, never having to refresh.  

With everything stored in the state, there's no need to fetch the entire database every time you want to load the list of articles.  The only thing that's required is deleting or adding to the state, and making a single fetch request to reflect new changes in the database.  That request would happen in the background and not interrupt the flow of the page.  

If I don't count the learning of Redux as part of the building process, then I moved from the backend to the creation of React components, and only when I was ready, built the store.   Every time I would make an action, it would be mirrored by a reducer case.  

I used React to design the containers and display of all data on the page, but for the most part, it felt like creating an app with Javascript.  React adds a lot in terms of ease of coding, but functions similarly to the way Javascript manipulates data, and the dom - in this case the virtual dom.  React also uses components which can either be functional/stateless or class components.  Class components must implement methods differently, with a render method, and any number of option lifecycle methods.  These proved to be useful in certain components.  

In the end, the project put everything together that I had learned, and I was proud that it could allow the user to use most CRUD actions with articles and comments.  Resembling reddit or wikipedia, I could see myself expanding on the app more in the future to add more user friendly features, such as search functionality, likes (which I never ended up getting to), or other ways to organise the set of comments and articles.
