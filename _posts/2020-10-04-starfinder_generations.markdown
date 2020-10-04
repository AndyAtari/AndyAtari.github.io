---
layout: post
title:      "Starfinder Generations"
date:       2020-10-04 16:53:27 -0400
permalink:  starfinder_generations
---


   When designing an app you want to explore strange new worlds and boldly go where no one has gone before, but before you set off into space you need to create some boilerplate code. The initial setup of an application can be daunting and tedious but it’s necessary to get your app up and running. So how do you go from idle to warp speed in development? Ruby Generators! Ruby on Rails provides an extensive list of generators that will write core application functionality code for you. That means development will be faster, more consistent, and you will not need to worry about memorizing repetitive code. This is a powerful tool for any Ruby developer. 
 
	  To explain Ruby generators, I would like to share some common and valuable generators I used to create my Starfinder Companion App. The one generator I did not use and advise to use with caution is the ```$ rails generate scaffold```. This command will create a full set of MVC code and a whole lot of unused code/directories. Although this command can instantly get your app running, you will most likely spend more time going through all the unnecessary code then if you just wrote the boilerplate code yourself. It may also cause you excessive bugs and headaches later on so I would just avoid it for now. Also, all these generator commands were used after the initial ```rails new``` which you should use to create an entire rails directory structure. 
	
	  Some early on generators I used were model and controller. It is very easy to type these commands in your terminal. Say I wanted to create my Starship model, I would write ```rails generate model Starship name:string tier:string```. This would generate a Starship Model file, a database starships table with a name and a tier column, and some associated tests. The model generator creates only a few necessary files to give you ultimate flexibility. You can also save time by typing ‘g’ instead of ‘generate’ and just typing the column name since string is the default type. So, in my terminal I would have typed ```rails g model Starship name tier```. A controller generator would be similar with the emphasis on controller. If I generated ```rails g controller Starship index```, I would get a Starship controller with an index method, routes for each action (in this case index route), and corresponding starships view folder and helper files. It would not generate a model or table migration. Both are useful options, but wouldn’t it be nice if we could generate all the above?
	
	  My personal favorite generator for Starfinder Companion was the swiss army knife of Ruby generators, ```rails g resource```.  With that simple command a model, controller, database table, view directory, helper directory, test suite, and styling files are created within seconds. So when I added starships to my application, I added the command line ```rails g resource Starship name tier``` and I was all set to start coding. I could start thinking about how starships related to other models and how the user could interact with starships. It gave me more time figuring out the purpose of my app and less time writing repetitive boilerplate code. 
	
	  Perfect, the ship is ready to take off and you now understand all the rails generators! Well not quite. There are numerous generators including ```rails destroy```, which is the opposite of rails generate and will destroy any generation you don’t need anymore, and even custom made generators through ruby gems or your own creation. There is also one other specific generator I used often in my Starfinder app that I would like to share, ```rails g migration```. This handy command will create or alter a table in your database and will automatically assign it a timestamp. Here are some examples of common migrations I used:
	
```rails g migration CreateCharacters name``` - This created a characters table with a name column with a string type.
```rails g migration AddUserIdToCampaigns user_id:integer``` - This added user_id column with an integer type to the campaigns table.
```rails g migration RemoveStatusFromCampaigns status:Boolean```  This removed the status column with a Boolean type from the campaigns table.
	
   As you can see there are many options for generating migrations, and I highly recommend practicing creating tables and altering columns this way to make you a more efficient programmer.
	 
	 With Ruby on Rails generators you will no longer be left in the cornfields looking up at the stars. The speed and efficiency of ```rails g``` will take your application to the final frontier. 

