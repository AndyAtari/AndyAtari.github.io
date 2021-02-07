---
layout: post
title:      "React/Redux Final Project: Building My Foundation"
date:       2021-02-07 18:12:18 +0000
permalink:  react_redux_final_project_building_my_foundation
---


My time as a Flatiron student is coming to an end, but my career as a software developer is just beginning. This transition has made me think about my career goals and what I personally want to achieve as a software developer. I will soon post a blog about my computer science goals for 2021, but for now I want to reflect on my workflow and how I can improve it for maximum productivity. Let me share with you my process of frontend setup with “An Animator’s Dozen” and what I learned about my initial workflow.

I like to approach my software development projects like I’m building a Lego house. I need a Lego baseplate before I start building my house, and then I need to lay the foundation bricks before I start building vertically. My baseplate for my Redux project was index.js. This file imports our App.js component and tells React where to render it. Essentially, index.js gets the element of root and inserts your App.js into the index.html. This approach enabled me to start coding and testing a React app right away without touching the index.html file. It is fantastic, and it speeds up my workflow. 

At this point, my baseplate is set but it’s a little thin. I can strengthen it by stacking another baseplate on top. The second baseplate is not completely necessary, and I could strengthen my project through other means later in my workflow. However, I already know that I will need some additional imports later in my project, and I can go ahead and add them now. Most of these imports pertain to Redux. I imported reducer, provider, createStore, compose, applyMiddleware, thunk, and logger. These imported files and middleware set me up for success later in the development lifecycle by assisting me in debugging and writing DRY code. This becomes super important when you push your project to github so others can easily find, read, and contribute to your code. I highly suggest further research into Redux middleware (or at least hover over the description in VSCode). 

Now it’s time to start stacking bricks. These bricks come in the form of Routes and Components in App.js. This part of my workflow ranges from easy to difficult depending on my level of project planning. I quickly learned that if I don’t project plan or my plans change, then my App.js starts to evolve or get really messy. I need to be conscious of my overall user experience and interface in order to avoid unwieldy code. I decided on 4 routes (“/”, “/q&a”, “/upload”, and “/login”) and imported a container for each route and a fixed header component. This is my function App:

```function App() {
  return (
    <div className="app-container">
      <Router>
        <Header />
        <Switch>
          <Route exact path="/" component={HomeContainer} />
          <Route exact path="/q&a" component={QandAContainer} />
          <Route exact path="/upload" component={UploadContainer} />
          <Route exact path="/login" component={LoginContainer} />
        </Switch>
      </Router>
    </div>
  );
}```

It’s clear and concise, and I know exactly what I will need to build for my project. With that my foundation is set, and I’m ready to start coding (a process that will take many many hours).

A little sidebar for you: I also recommend a few fun VSCode extensions that simplify initial setup and help keep you zen throughout your JavaScript project. ‘Prettier’ will make your code more attractive and legible, as the name suggests. It auto formats your JS so that you don’t have to participate in the spaces vs tabs war. ‘Bracket Pair Colorizer 2’ colorizes your curly bracket so that you don’t get confused on where your functions begin and end. ‘Panda Theme’ is a fun dark mode theme; it's just a personal preference, but it looks cool and the colors are fun!

So what did I learn about building my programming foundation? For starters, I learned that without project planning, I just end up staring at my baseplate. I need to spend even more time on project planning going forward, and it’s a skill I would like to build in 2021 and beyond. I also learned that once I have my initial foundation set in place, I can start envisioning my project and what components I want to create/work on first. I need those first few coding bricks so I can start building out my house and adding features and decorations to my new home. I have the desire to build a beautiful project, but without a strong foundation it will all fall apart.

