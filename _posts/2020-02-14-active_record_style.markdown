---
layout: post
title:      "The Purpose of Active Record"
date:       2020-02-14 22:50:25 -0500
permalink:  active_record_style
---


Active Record is an important step in accessing backend data written in SQL.  It can be seen as the model in the MVC paradigm.  Modeling data should be used whenever many of one type of object will be created, or managed by the user.  Without the involvement of a user in object creation, objects would be made without Active Record and stored in Ruby or SQL if there are many.  Active Record allows for easy creation and retrieval of information stored in SQL databases without the need for SQL code.  All the methods that the user has access to allow for this to happen by extending Active Record into new classes that will retrieve or create objects and data.  

I believe Active Record should be used whenever the creation and maintanence of data outpaces what is already accomplished without any user intervention or what is accomplished by the user alone.  Basically, whenever data is getting accessed quickly, Active Record should be used to save time in writing code, and using SQL commands unnecessarily.  It's easier to read and understand as a coder who is reviewing code, and it's easier to write and manipulate objects with for coders themselves.
