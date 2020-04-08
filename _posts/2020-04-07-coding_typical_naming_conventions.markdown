---
layout: post
title:      "Coding Typical Naming Conventions"
date:       2020-04-07 19:57:11 -0400
permalink:  coding_typical_naming_conventions
---


While creating an app of any type, it's good to keep a consistent system for naming variables, databases, classes, and methods.  Most naming conventions come down to camel casing, snake casing, or pascal casing.  Naming conventions with apps that have both a front and back end, and controllers in the middle, should be particularly careful with naming conventions as the complexity of the project increases.

For classes the default in most apps is Pascal casing.  This means that the first letter of each class name is capitalized as well as the first letter of each additional word in the name. 

Camel casing seems to be used less frequently than Pascal casing, but it can be used for local or global variables.

Database columns, names, migrations, as well as local variables often use snake casing.  This means that words are lowercase and separated by an underscore, making each very visible and easy to read.  Another usage of snake casing in typical sinatra apps is for file names.  Regardless of the name of the class within the file, the file itself should be snake cased.  

This method of naming extends to the creation of migrations, as the command to create a migration is rake db:create_migration NAME=tablename.  The resulting migration will automatically be made as a class named CreateTablename, using Pascal casing.  The name of the table should always be the plural of the model that it contains.  For instance if you make a model called user, the class name should be User, the table name should be users, the rake command to create the migration should be create_users, and the created migration class should be CreateUsers.  That's 5 different names for dealing more or less with one object.  Luckily a lot of that is automatically created thanks to Rake!  

It's probably a good habit to check that the automatically created files are consistently named if for no other reason to proofread the code for mistakes.  The most important part about naming conventions may come down to others being able to read your code without being thrown off when the project requires more than a single coder's work.



