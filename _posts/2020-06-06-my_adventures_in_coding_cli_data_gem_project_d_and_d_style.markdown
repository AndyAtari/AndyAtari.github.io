---
layout: post
title:      "My Adventures in Coding: CLI Data Gem Project (D&D Style)"
date:       2020-06-06 12:47:08 -0400
permalink:  my_adventures_in_coding_cli_data_gem_project_d_and_d_style
---


As I sit here at my computer desk, with my Baby Yoda figurine watching over me like an encouraging mentor, I think back on the process of creating my first portfolio project for Flatiron and for my new career. It began with an idea that became another idea that became another idea….well you get where I’m going. Project planning is a mountain in itself, and I was determined to climb it no matter how long it took me. When I discovered the Dungeons and Dragons API, I immediately knew I could create a fun and rewarding CLI from the data. 
	
	I wanted to create an application that would display different Dungeons and Dragons (D&D) character options and give the user enough information to create the most epic character. I originally wanted to go many levels deep and return all the data on character creation. I have never played D&D, but I have played enough role-playing games to know that would be a daunting task. I started thinking in terms of MVP (minimum viable product) and decided to start with the foundation of character creation: choosing the character’s race. My CLI returns stats on each race that the user is interested in. It is a fantastic start to my CLI. 
	
	I first created my GitHub repository and then worked on creating the essential files and folders for my project to work. Next, I created an API get request and iterated over the data so I could find the race names and display that list to the users. All of this seemed comprehendible to me until I had to verify if the user’s input was valid. My goal was to create abstract code that was not hard-coded. After much trial and error, I ended up using each.with_index() and corresponded each index with a race name. From there I could use my find_by_name method and not only verify if the name was an actual D&D race name, but I could also pass that name as a parameter for calling my second API get request. After that, it was all gravy! Well, not exactly...I often found that by changing one method I would have to refactor other methods just to make my code work again. For example, when I implemented the to_i method I forgot that the method will take a letter or word string and return 0. That led me to refactoring my code to account for a user accidentally entering a letter key. I wanted to make sure my interface worked first and foremost but also wanted concise and DRY code. I wanted it all!
	
	Looking over my project now, I have a working CLI that is user-friendly and fun to use. Is my code perfect? Absolutely not! But that is the purpose of this course: to refine my coding skills over time. My code has come a long way. I am polishing up aspects of it and refactoring methods to make it more abstract. I know that I learned a great deal over these past few weeks. I also know that I still have much to learn, but as the older Yoda would say, “Much to learn you still have, my young padawan.” 

