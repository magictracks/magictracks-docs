# Updates and Notes

*Migrated from Github Issues to this single living document*


***
### 20180830
***

The last week of the summer - lots to do!

* Todo:
   - [ ] documentation for project developments from June 7 (start) to Aug 30 (end of summer)
      + [X] project roadmap
      + [X] project next steps (see below)
      + [X] key learnings and decisions
      + [X] project overview documentation - where is everything living / links / descriptions
   - [ ] tutorial maker web application front-end interface documentation and feedback
   - [ ] browser-plugin sync with web application interface
* next steps:
   - [ ] connect tutorial maker front-end interface to back-end database and API
   - [ ] connect browser plug-in to back-end database and API
   - [ ] application documentation - API, setup, etc.
   - [ ] initial testing and discussion of next steps

NOTE:
* I'm away starting Aug 31 - Sept 15. I will be mostly offline, but happy and able to answer questions while away.

## Project roadmap - up until today: Aug 27, 2018

![paper itp hacking higher ed 27](https://user-images.githubusercontent.com/3622055/44663661-29ddc100-a9df-11e8-9d68-bac59d01de26.png)

## Key Learnings & Decisions

(just going to steam of consciousness right now, will group and saturate later)

> We need the "mortar to the bricks"

This was a key insight - the internet has already an endless amount of resources, how we bring them together in an intelligent and helpful way is the research question. We need to think deeper about the mechanisms that allow people to keep track of, share, build on top of, branch and fork from, and improve teaching materials

> Landing on the right technologies

It took awhile for me to decide which tools and technologies feel right for these particular projects. I've been trying to keep in mind the balance between:
* project readability (can the code and the various design and software decisions be deciphered in a logical and structured way?),
* approach-ability (at what level of expertise do people need to have in order to jump into this project - does that determine whether it will live or die?) ,
* and usability (do we build our own custom solutions or try to bend our solution around existing platforms and services?)

I tried to conjure up my own raw html5 solutions (it was an interesting exercise) using object oriented programming (OOP), but that couln't handle the project scope/needs, despite probably being the most easy for people to jump into if you're just learning OOP structures in javascript. State management is tough!

Then on the complete opposite end, I spent some time trying to build some proofs of concepts with React/Mongo/Node/Express and also Next.js which is a wrapper around the React.js framework. Adding things like Redux and trying to keep track of that whole environment did not seem conducive for collaborations outside of those who are deep into those frameworks. They have their merits, especially Next.js seems pretty cool, but still did not seem to fit the balance mentioned above.

Enter Choo.js and Feathers.js: Yes, all these web frameworks will live and die, but I feel happiest about these two. Choo.js is a lightweight front end framework. Similar flavor of React in which your write components, but state is accessible from everywhere and it's all native dom elements. To say the least, I'm very happy with it!

Feathers.js is probably the closest thing to waving a wand and saying, "build me a web app with REST API endpoints. That being said, there's still a few things that take some time to figure out, but it is probably one of the more approachable and prescriptive (in a nice way) back-end setups.

> Build the thing

I spent a lot of time this summer learning new things by exploring alternatives to our own home grown custom web app software solution. I learned to use things like localStorage for offline data storage and OAuth from other applications to handle authentication and hack github issues for example to be a kind of "database" (I need to publish some of those experiments at some point). I think it took all of those experiments to get to the point I'm at now, so in that sense that time has been indispensable. I do also think though that it is useful to build out a version of "the thing", whatever it is, even if it will never see the light of day or if we decide as a team not to keep going with it, so we have the choice in the first place to continue with the project or not. The key thing being to document the learning and software so we can pull out the little bits of gold for later projects. Anyhow, I'm feeling pretty good about building up this first version of the [magic tutorial maker - tenative name]() so we can see if/where to take the project next.


**more soon**


# Project overview documentation

## [itp-diy-syllabus](https://github.com/joeyklee/itp-diy-syllabus)

This has become the repository containing the project documentation. Along with the [/concept](https://github.com/joeyklee/itp-diy-syllabus/tree/master/docs/concept) and [/wireframes](https://github.com/joeyklee/itp-diy-syllabus/tree/master/docs/wireframes) for the initial concept explorations, the [update/concept issues](https://github.com/joeyklee/itp-diy-syllabus/issues) are some of the main source of project documentation and progress across all of the related project repositories

NOTE: It will be a good idea to migrate all of the project specific info to their respective issues, etc.
NOTE: for convenience in the future, I think I might keep all of the update/notes in 1 issue but under different comments rather than blowing up the issues.

## [itp-tutorial-maker](https://github.com/joeyklee/itp-tutorial-maker)

<img width="685" alt="screen shot 2018-08-27 at 11 01 53" src="https://user-images.githubusercontent.com/3622055/44667384-a6c16880-a9e8-11e8-8eb9-9aa4a0fcb1a8.png">


The itp-tutorial-maker repo is the web app - front/back end - of the tutorial maker.

## [itp-resource-collector](https://github.com/joeyklee/itp-resource-collector)

The itp-resource-collector is the repo containing the project for the browser extension. This might make more sense living in the same repo as the tutorial maker and may be migrated. This is TBD



***
# Deprecated

A bunch of repos that were spun up that might be archived. TBD.

## [itp-tagged-resources](https://github.com/joeyklee/itp-tagged-resources)

A repo that was used for experimenting with usign Github as a sort of API / issues == database. No longer used at the moment. Maybe there's a productive use for this idea/concept later?

## []

## [itp-resource-collector-api](https://github.com/joeyklee/itp-resource-collector-api)

Repo containing that was once used as the backend for the itp-resource-collector. Since we are using the itp-tutorial-maker for the client and server for the project space, we should move any handy scripts from here over to the itp-tutorial-maker repo

Some of these handy scripts include those for:
- [ ] downloading the coding train video data from youtube's API
- [ ] sorting and grouping the coding train videos based on tags

***

# not project related but relevant to know

## [itp-office-hours](https://github.com/joeyklee/itp-office-hours)

This is a repo for improving the ITP help desk, specifically the issues around booking office hours, etc. The repo contains the generator scripts for getting all the current faculty/staff/residents with office hours and grouping and suggesting alternative expertise them based on text similarity.


## updated tutorial making/editing screen

### in the style of what you see is what you get
![screenshot_2018-08-30 client - edit](https://user-images.githubusercontent.com/3622055/44880550-ca9bdd00-ac7a-11e8-969e-3641eacf3e3d.png)

### click through form

![screenshot_2018-08-30 client - edit 1](https://user-images.githubusercontent.com/3622055/44880598-e99a6f00-ac7a-11e8-8acb-d5d3c04aca53.png)



***
### 
***
