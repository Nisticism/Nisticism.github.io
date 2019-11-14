---
layout: post
title:      "City Scraper CLI Project"
date:       2019-11-14 23:12:24 +0000
permalink:  city_scraper_cli_project
---


The creation of my first project in Ruby combined many things I've learned throughout the course.  It started by creating the file system of the project.  It's important to stay organized in programming and not get too ahead without adequate testing.  I needed to create the necessary folders before anything, so that all the other steps would be made easier.  The bin folder held the executable file to start the project.  The lib folder holds all the classes to run the program, including the CLI itself, the scraper, and the objects made from the scraped data.

Scraping was still relatively new to me at the time, so it took a little trial and error to select the right elements that were displayed in Javascript on Wikipedia.  I needed to select the css only with the Nokogiri gem that already helped parse through the javascript.  There were two main selections - the page that displayed all the cities, and the details page that selected the descriptions of each city.  I had to iterate through first the tables, then the rows, and finally each element in each row.  

The CLI building was not difficult because I knew it was a matter of displaying the menus and making sure the user could navigate them without a problem.  This can be done using a loop.  Is the selection valid?  Yes?  Okay run the method that displays whatever the user wants from the menu.  No?  Just run the menu again and ask for another selection.  At any point the user can exit the program.  After seeing a list, pressing any key returns to the main menu.  

I learned a lot about scraping, and further uses for object oriented programming, as well as the Ruby language.  The Has-Many relationship can be useful when several cities have the same country.  I was able to create both City and Country objects from the data I scraped using Nokogiri.  Feel free to check out the city scrape code that's in my github.
