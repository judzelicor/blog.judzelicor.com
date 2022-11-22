---
layout: post
title: "Why I Started Using Vite For My React Projects Instead of CRA"
readtime: 12
description: "A brief talk about Vite, what its significance is in React projects, and why you should use it in your next project instead of React's create-react-app toolchain. Warning, the writing might include a bit of dramatization."
categories: ["programming"]
---

<h3 class="sectionTitle">Introduction</h3>

In my early days of learning React, I was acquainted with a tool called <span class="terminology">Create React App</span> or <span class="acronym">CRA</span> that allows beginners to setup a React project without learning how to configure bundlers such as <span class="terminology">Webpack</span>. It was like magic. All I had to do was type into my terminal these words
```
yarn create react-app
```

And after several minutes, the ritual would be complete, and I was good to go. But as I countinued to hammer on my keyboard, I couldn't help but notice how heavy my fingers felt with each character that I typed. Was it truly okay for me to have enough time to prepare dinner, do my skincare routine, watch the new episode of Demon Slayer, and complete a medium Leetcode question, depending on how fast my internet connection was on any given day before I could start coding? Am I doing the right thing? Was I truly... happy? 

Even to this day, I'm still unsure of whether it was the tomato juice that I drank during the ritual that was talking, but those idle thoughts kept me from being productive. It consumed me and I thought I had to do something.

I was browsing Reddit one day, just like any other day, when I came across a post. It was your typical "either or" question. "Vite or CRA", the title read. My heart reverbarated as if it was the first time that I've had exercise in weeks and before I knew it, I was browsing the comment thread.

<h3 class="sectionTitle">What is Create React App?</h3>

Traditionally, before you could start using React, you need to write a configuration file for how you want your project to be bundled. In other words, you first have to learn enough about <span class="terminology">bundlers</span>, <span class="terminology">transpilers</span>, and other jargon just so you could render your a text that says "Hello World" in React.

While it might sound worthwile to learn new things, at that point, there's no concrete reason to tinker with those concepts yet as they aren't needed to practically learn React. This is where create-react-app comes in. It allowed programmers of all levels to quickly start a project without having to write their own configurations. The team around React wrote configurations with maximum compatibility with any kind of project idea. From a todo list app to your own <span class="acronym">SaaS</span>, create-react-app can speed things up especially if your purpose is to create a proof of concepts before you build the real deal with your weapon of choice.

However, as it stands, when your weapon of choice is create-react-app, you have to deal with the fact that it's slow the more ambitious your project is. A larger project size lead to performance bottlenecks especially for projects built with Javascript tooling because inherently and relatively, Javascript *is* slow. In my experience, even with <span class="acronym">HMR</span>, it can take a couple of seconds before my changes are reflected on the browser after making an edit. It can take minutes too just to setup a proper working development server with create-react-app. All these inconvenient instances will compound one after another and begin to affect my productivity. 

That is why I began my research of finding an alternative and luckily I wasn't the only one feeling this way and brilliant programmers have created a solution that solves all these problems and more!

<h3 class="sectionTitle">What is Vite?</h3>

Vite, just like create-react-app, is a tool that aims to streamline the creation of your React projects.

<h3 class="sectionTitle">How to start using Vite?</h3>
Starting a new React project with Vite is simple.

with NPM:
```
npm create vite
```

with Yarn:
```
yarn create vite
```

After that, just respond to the prompts and let Vite handle the initialization of your React project for you.

<div class="articleNote">
	<div style="width: 18px; fill: #fef3c7; margin-top: 3px;">
		<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16">
		  <path d="M6.5 13.5h3a.495.495 0 0 0 .5-.5v-1.9a5.5 5.5 0 1 0-4 0V13a.495.495 0 0 0 .5.5zm3 1.5a.5.5 0 0 0-.5-.5H7a.5.5 0 0 0 0 1h2a.5.5 0 0 0 .5-.5z"/>
		</svg>
	</div>
	<div>
In my experience, whenever I start a Vite project with yarn, I get a warning something along the lines of "vite: command not found". If you encountered the same error, just run <code>yarn install</code> or <code>yarn</code> first and you should be able to start your project with <code>yarn dev</code>.
</div>
</div>