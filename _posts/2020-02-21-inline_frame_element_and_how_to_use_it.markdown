---
layout: post
title:      "Inline Frame Element and How to Use It"
date:       2020-02-21 16:35:47 -0500
permalink:  inline_frame_element_and_how_to_use_it
---


The Inline Frame Element or <iframe> as it appears in code, is a designation of a nested browsing context.  

Each nested browsing context has its own session history and document.  The context that embeds other nested contexts is called the parent, and the top most level is usually the browser, and represented by the Window object.  

There are a few specific cases when it's better to use iframes than other options.  If you need to section off a piece of a website because it has its own function that is distinctly different from the rest, such as mapping the location of a building, an iframe might work.  It should not be used to display common objects such as photos, as other tools are better suited for that purpose.  
