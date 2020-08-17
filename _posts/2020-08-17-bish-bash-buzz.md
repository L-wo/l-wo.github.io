---
layout: post
title: Bish Bash Buzz
subtitle: "My first 'proper' web application!"
date: 2020-08-17 22:00:00 +0100
background: '/img/posts/07.png'
---


#### [http://bishbash.buzz](http://bishbash.buzz)

So, this is my first web application to be released into the wild. I built upon the knowledge I gained with *Marvin Rigs It All* and learned a lot of new skills too.

We have been enjoying a lot of Zoom Quizzes (video conference quizzes) during lockdown and we were trying to think of ways to spice it up a bit. At the time of writing, my good friend Steve has written **20** quizzes for us without taking a week off! Each week a group comes up with a bonus round - usually the format is a bit different and uses video, music or images to create something a bit different.

This gave me the inspiration to build *Bish Bash Buzz*, a quiz buzzer web app. There are several others out there doing a similar thing, but each one has enough quirks I don't like (ugly UI, sign-ups, trying to do too much at once) to justify building something myself. I don't believe there is a viable business behind the app, more that it's a simple enough concept that I can complete and use as an experiment to find holes in my skillset and experience some new-to-me technologies.

Features include:
- Multiplayer quiz buzzing experience with very spacious rooms
- Easy host controls including setting modes and changing the state of the room
- Emoji based 'flair' and colour choice for each player

I deployed, as with my *Marvin* scoring system, on Heroku. This is a slightly more advanced deployment as it contains my first use of REDIS, an in-memory database. After building the prototype using in-memory storage, I decided to learn to use REDIS as a useful excersise and perhaps in advance of exploring horizontal scaling further down the road.

This was a great opportunity to get really hands on with websockets, specifically [socket.io](http://socket.io). The whole thing is structured around a socket connection. I won't lie, I'm not happy with the structure of my express app for this project. Getting bogged down with where the business logic, data access and socket message logic sat encouraged me to do a lot more reseach on how people structure their applications. As a result, my latest project is using a much more ordered layered approach I am much happier with.

I've also massively improved my workflow, using [npm-watch](https://www.npmjs.com/package/npm-watch) to automate various tasks like obfuscation and sass compiling. I'm feeling more confident using VSCode and am finding more and more shortcuts each day.

I last touched this project about a month ago, having finally secured some genuine paid development work (which I will write about soon!) but I am hoping to return to it in my spare time.

Why not give it a try next time you are hosting a bonus round? [Bish Bash Buzz](http://bishbash.buzz)



