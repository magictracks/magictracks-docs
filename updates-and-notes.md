# Updates and Notes

*Migrated from Github Issues to this single living document*


***
## 20180830
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
##  20180823
***

Hi All,

Just writing a quick update for now. I've spent this week learning about [Feathers.js](https://feathersjs.com/) - a pretty neat wrapper around node/express - and figuring out what it would mean to connect it up to [Choo.js](https://choo.io/) for our frontend.

I created a boilerplate: https://github.com/joeyklee/feathers-choo-boilerplate to start thinking about some generic setup for making apps in the future.

I've been getting some tips from @blahah who is helping me to setup Feathersjs and Choo using best practices for both frameworks.

In tandem, I've been trying to quickly start building out the front-end of our Magic Tutorial Maker (see screenshots below) so when the backend is setup, I can connect it all up. The development is happening on the `client-refactor` branch: https://github.com/joeyklee/itp-tutorial-maker/tree/client-refactor

@matamalaortiz any ideas or feedback would be cool on interface considerations or other things you think would be good to see!

Here's some screenshots so far, but I still have a lot to do to flesh out all of the screens:

## Landing page:

![screenshot_2018-08-23 client - main 1](https://user-images.githubusercontent.com/3622055/44547219-644a1400-a6e8-11e8-8396-f8cd5fe22f26.png)


## Login modal:
![screenshot_2018-08-23 client - main 2](https://user-images.githubusercontent.com/3622055/44547226-690ec800-a6e8-11e8-900c-afb11e0fd682.png)

## browse page:

little boxes indicate number of sections + resources within each section

![screenshot_2018-08-23 client - browse 4](https://user-images.githubusercontent.com/3622055/44555501-7be2c600-a703-11e8-894f-3d61f56e8508.png)



## create page for overview of works

little boxes indicate number of sections + resources within each section

![screenshot_2018-08-23 client - create 1](https://user-images.githubusercontent.com/3622055/44555463-52299f00-a703-11e8-8f25-dad4ee2460f4.png)


## Search page

![screenshot_2018-08-23 client - search 1](https://user-images.githubusercontent.com/3622055/44555443-37572a80-a703-11e8-8ffa-c625a60907c7.png)



***
## 20180816
***

Developing on the thoughts from #29 around better integrating resource tagging and the tutorial making, I decided to re-write the [Resource Collector browser plugin](https://github.com/joeyklee/itp-resource-collector/tree/master/browser-extension) keeping in mind that it would be nice to be able to add the resources directly to tutorials from the plugin itself without having to go to the main webpage for editing.

Here's the progress so far

## Upon opening the extension, a user authenticates/logs in w/ github auth

<img width="1550" alt="screen shot 2018-08-15 at 18 34 59" src="https://user-images.githubusercontent.com/3622055/44176996-187ce680-a0ba-11e8-9679-edb841796a71.png">
<img width="1550" alt="screen shot 2018-08-15 at 18 35 08" src="https://user-images.githubusercontent.com/3622055/44177007-1d419a80-a0ba-11e8-95d6-f961de20b9c5.png">

## Then user selects an image for the cover image
<img width="1333" alt="screen shot 2018-08-15 at 18 28 19" src="https://user-images.githubusercontent.com/3622055/44177029-27fc2f80-a0ba-11e8-92ec-1c551ca12d5f.png">


## user can edit or add tags, description, etc

<img width="1333" alt="screen shot 2018-08-15 at 18 28 23" src="https://user-images.githubusercontent.com/3622055/44177061-419d7700-a0ba-11e8-983a-1ecb9c1a0634.png">

## user then can organize into tutorial and section. If desired they can also add a new tutorial or section

<img width="1333" alt="screen shot 2018-08-15 at 18 28 31" src="https://user-images.githubusercontent.com/3622055/44177080-57ab3780-a0ba-11e8-8012-9d54a86d4fce.png">
<img width="1333" alt="screen shot 2018-08-15 at 18 28 39" src="https://user-images.githubusercontent.com/3622055/44177081-57ab3780-a0ba-11e8-94d4-61950092ff22.png">

## Todos:
* Nothing is hooked up to a backend service yet, but that's the plan the next couple days.
* needs better multi-select interaction for tags
* create integration with tutorial maker / open new tab ==> with main Magic tracks webpage
* no styling applied yet, def. need to do this as well


## Updates: 20180817

Hello! So my major update is that I spent a bunch of time to map out the workflow that needs to go down using our own homegrown system. I've been discussing with a friend @blahah and he has helped to define some data models and considerations for how to keep this thing running in a nice way.

I've diagrammed out what the next 2 weeks are going to look like in terms of building stuff out. By working through this workflow - setting up the frontend and backend for the web app, and browser extension - and integrating some of hte design proposals from @matamalaortiz - I think we will have an initial workflow to get the conversation going about how we might start to rapidly create learning materials from a set of vetted resources.

see:

## auth workflow

![paper itp hacking higher ed 26 2](https://user-images.githubusercontent.com/3622055/44290889-e6e65580-a248-11e8-8342-b390c9f6573c.png)


## for browser extension

![browser-extension-workflow](https://user-images.githubusercontent.com/3622055/44290896-f9608f00-a248-11e8-9068-ab0246303d1f.png)


## for Web app

![web-app-workflow](https://user-images.githubusercontent.com/3622055/44290897-f9608f00-a248-11e8-9341-62f78a43c574.png)



***
## 20180809
***

Hello!

This week, I jumped right into development and have been building out our [Tutorial Maker](https://github.com/joeyklee/itp-tutorial-maker).

Updates:
* I'm using [Choo.js](https://github.com/choojs/choo) as a framework. I'm very happy with it as it is super readable, approachable, and takes care of the state management issues I was running into before. Super happy about it! There's def. some structural things I can improve on, but I like that Choo gives us a lot of flexibility to build and refine.
* Here's a quick demo of what we've got so far:
👉 https://www.youtube.com/watch?v=H8hFcfKR464&feature=youtu.be

![screenshot_2018-08-07 client-choo - main](https://user-images.githubusercontent.com/3622055/43806212-09bdd068-9a71-11e8-9e94-930548132c3e.png)

Maybe @matamalaortiz and I can have a chat about UI this week?

Just had a chat with Kenzo on his https://subdex.co/ project. Really a cool one around social link sharing. We might consider to loop in or integrate with his efforts if it makes sense for us.

https://subdex.co/about
> Share with friends interesting sites you've found on the internet, know what resources educators recommend for learning a subject, and follow what subject matter experts are reading.

Really nice core features of Subdex:
* link suggestions for lists of other people ==> imagine you see that someone wants to learn CSS and you can suggest links for them
* organization of links into subsections
* forking of lists & collaborative lists
* sorting and filtering by tags
* list ownership as a way of maintaining lists

Some features that might be interesting for him that we've had in mind is to do better job at linking posts through text analysis. Also, a browser extension would be cool to send links to your own lists.

![screenshot_2018-08-08 subdex discover follow and create lists of links](https://user-images.githubusercontent.com/3622055/43860338-6338ed5c-9b21-11e8-9b54-f6efa352ac8a.png)

# Updates 20180809

Features implemented this week:
### Input/output
* Open JSON file:
   - open a structured json file locally and continue working/editing your tutorial
* Open from local storage:
   - open structured json from your local storage and continue working/editing your tutorial
* Save to localStorage:
   - save your tutorial progress to localStorage so you can continue working (not meant to be the primary mechanism for saving since your localStorage can disappear, but rather for within browser sessions)
* Save as JSON:
   - export your tutorial as a structured JSON file
* Save as HTML:
   - export your tutorial as a styled HTML page to embed and use elsewhere on the web or hosted e.g. in GH pages. (still lots of styling to do and features to add - but proof of concept is working)



### Editing:
* Editable Tutorial titles/descriptions
* Add your own image from your filesystem by converting to base64
* Adding sections and resources
* Editable Section titles/descriptions
* Reordering sections and resources
* Deleting sections and resources

The tool can work entirely offline at the moment. We however will need the web to connect to our tagged resource db & to be able to save, store, and host tutorials online. Also now after working with the tool, it would be rad to save the sections (conceptual building blocks / resource containers) to be able to copy them across tutorials.

## Example images

![20180809-prototype-rendered-view](https://user-images.githubusercontent.com/3622055/43922350-7bd208be-9bec-11e8-9bbe-a0ca9264dd73.png)

# 20180810: Thoughts

I decided to take some time today to step back from coding and evaluate where we're at at this point.

In general we're trying to work through this loop:

## Collect > Tag/Enrich/index > (re)use / remix / reference > share > feedback
![paper itp hacking higher ed 23](https://user-images.githubusercontent.com/3622055/43984193-0fafedcc-9ccd-11e8-8df8-809245050321.png)

## Collect > Tag/Enrich/index

Here, we collect resources via manual tagging from people and also ones that are added by people creating lists and lists of lists or tutorials

We enrich / tag / index these references by automated and human means to try to make it easier to find stuff. The idea is that the people submitting to our database

![paper itp hacking higher ed 22](https://user-images.githubusercontent.com/3622055/43984216-34f1c34e-9ccd-11e8-821a-7fcc3667bda2.png)

##  (re)use / remix / reference

We want to ultimately encourage use, reuse, remixing, and referencing of all the great resources that exist out in the world. We also want to try to make it easier to quickly put together lists of references in an organized way for people (e.g. students) to address learning on a per project basis.

Collaboration is really important here

![paper itp hacking higher ed 23 2](https://user-images.githubusercontent.com/3622055/43984268-849280e6-9ccd-11e8-9e74-c3eafb3ba92f.png)


## Share

We want to encourage easier and better sharing of learning materials through collaboration and having a way to better highlight the creation and organization of materials

![paper itp hacking higher ed 24](https://user-images.githubusercontent.com/3622055/43984308-b975b35a-9ccd-11e8-8a5b-a068b526538e.png)

## Feedback

As educators it is helpful for us to have feedback about learning pathways that work or don't. Sometimes it helps to do less, somtimes we need to do more. Having ways to incorportate and track feedback and growth is important

![paper itp hacking higher ed 26](https://user-images.githubusercontent.com/3622055/43984343-faa9a73c-9ccd-11e8-89aa-a66adfbcf208.png)


***

All that being said, I wanted to take a moment to also evaluate what is working in our current thinking, what similar products exist out there, and what things we might continue referencing to help us guide ideas around seemlessness and ease of use.

## What's happening now:

So right now we have an proof of concept for collecting and storing resoruces to a central db via a browser extension. This is our first touchpoint with adding and collecting information to a database from which we can pull from regarding references like coding train videos, etc.

![paper itp hacking higher ed 17](https://user-images.githubusercontent.com/3622055/43984395-5f510e78-9cce-11e8-94a5-e62f19b21169.png)

In the pursuit of creating tutorials with these references pulled from the web, we can also create references from our tutorial maker (not yet implemented). This I think makes sense since it doesn't feel great to only be able to submit references using an extension. We def. need multiple ways of submitting to the knowledge base.

![paper itp hacking higher ed 18](https://user-images.githubusercontent.com/3622055/43984425-8ed81f92-9cce-11e8-8381-bcc0797546ce.png)

So far, nothing special - there's heaps of products like Pinterest, dribble, Instructables, and more that provide similar endpoints for the materials gathered across the web + teaching people stuff or inspiring others. Even Subdex which is developed by ITP alums is about social link sharing, suggesting, and maintaining web links.

![paper itp hacking higher ed 19](https://user-images.githubusercontent.com/3622055/43984494-e9926104-9cce-11e8-9864-ffc6f010f7f2.png)


What will make our thing special is a kind of seemlessness that really makes it easy to collect, make, create, and curate resources whenever and wherever. I diagrammed some of the Pinterest workflow touchpoints that make that service quite nice. Not to say that we are building another pinterest - that would be v. hard - but I think it serves as a handy analog for making sure we don't skimp on the ability to allow for many ways of adding stuff, curating stuff, organzing stuff, and sharing stuff. Also, a good value added would be for exportability or interopability of the data produced. Keep. It. Open!

![paper itp hacking higher ed 20](https://user-images.githubusercontent.com/3622055/43984557-45639c96-9ccf-11e8-95d2-347bf5423397.png)

## Last points

In working through the pinterest workflow and given our progress on the tutorial maker, I think it is a good time to draw a stronger connection/integration between the tutorial maker and the resource collector. I will revisit this next week. For now, I've setup up a simple scaffold for using Choo.js as a framework for building our browser extension so we can maintain the readability across our applications. see https://github.com/joeyklee/itp-resource-collector/tree/v2/browser-extension

I will leave it here, and pick up on Monday. Ciao!


I decided to go back to Sketch and create a few new mockups. Sharing here some ideas for the Tutorial Maker View, output Tutorial View ( HTML version) and Tutorial Discovery view. @joeyklee this week we can discuss some ideas around this before I continue changing styles on my own branch. What do you think?
<img width="647" alt="screen shot 2018-08-12 at 2 06 02 pm" src="https://user-images.githubusercontent.com/5123955/44004973-962b64a4-9e39-11e8-88a9-f1cd13faa2b0.png">
<img width="632" alt="screen shot 2018-08-12 at 2 01 06 pm" src="https://user-images.githubusercontent.com/5123955/44004975-9e91140e-9e39-11e8-85ca-411d3c6a2b0e.png">
<img width="584" alt="screen shot 2018-08-12 at 1 56 24 pm" src="https://user-images.githubusercontent.com/5123955/44004978-a35e5c12-9e39-11e8-9e9d-5af3acf0a0e9.png">




***
## 20180802
***

Hello!

## Updates
* Currently working on building an interface for the tutorial maker tool (https://github.com/joeyklee/itp-tutorial-maker/tree/poc) | NOTE: on the `poc` branch
   - basic functionality right now includes: Adding a tutorial, adding sections, and adding resources to each of those sections. You can also get a representation of the data as json in the codemirror instance.
   - Current things I'd like to finish by the end of the week:
      + refactor code to work with data using LocalStorage rather than references to json objects floating across the app.
      + implement updating state across the visual and json editors
      + Make the visual editor more prominent
      + implement open/save file locally


![screenshot_2018-07-31 tutorial maker io 3](https://user-images.githubusercontent.com/3622055/43530309-43f2be6a-957b-11e8-802e-61285b30e43e.png)


***
## 20180728
***

Howdy to anyone/everyone who is tuning into these updates!

**Short note**: I was away this week participating in the Open Source for Open Scholarship (https://osaos.org/) workshop that was put on by Code for Science and Society (https://codeforscience.org/) and worked on the beginnings of an Open Scholarship Handbook - how to work openly in the context of education and research. In the next couple months there will likely be an alpha version of that handbook out in the world covering topics ranging from funding open source projects to operations and people management in growing open source projects. I'll keep you all posted on the progress there. In any case, it seems there is definitely interest in our efforts regarding the tooling and methodologies we're proposing.

## Project updates

I've been teasing out some ideas around what might be a method that will allow us flexibility to produce the content and visual output and structure we'd like, without getting too bogged down by heavy web app-y things that custom software solutions often require.

On the extreme end, I began trying out what it might be like to really build out a custom backend/frontend (https://github.com/joeyklee/itp-tutorial-maker/tree/client-refactor) and it already is starting to feel too heavy handed for what I feel we're trying to accomplish.

So after a few days away from the project, I poked my head around to for a project that felt like an apt analog for a lighter weight, highly functional tool for essentially editing data, storing it somewhere, visualizing it, and sharing it out in a number of formats and I landed on a tool I use quite a lot called Geojson.io - https://github.com/mapbox/geojson.io | http://geojson.io/#map=2/20.1/0.0

There's a bunch of things I love about this tool, but ultimately, I like that it is super easy to use, fulfills a very directed purpose, and allows you to easily bring in and create data and export and share that data across whatever relevant platform. In our case, instead of creating geosjson map datasets, we'd be creating the data to build tutorials. I will try to prototype a solution that is roughly modeled on some of the structural considerations and see if it yields something satisfying for us.

<img width="1438" alt="screen shot 2018-07-28 at 14 39 47" src="https://user-images.githubusercontent.com/3622055/43359676-2d6fbd00-9274-11e8-970c-d94ee9f7a704.png">

I'd like to focus this week on trying to see if I can create a proof of concept that allows us to have a better conversation about the direction things are moving in.

I'll post updates soon!

Some things to note:
* Anonymous gist creation is being deprecated: https://blog.github.com/2018-02-18-deprecation-notice-removing-anonymous-gist-creation/



***
## 20180713
***

Just a few updates from my side this week:

1. Started wireframing one possible solution for user flow of a more heavy handed software solution to bringing together learning resources: https://docs.google.com/presentation/d/1fxlmlrqK9ToM4nNNNKgsQFruHHxCQNwp97qA0woWZOA/edit#slide=id.p

2. Worked on Office hours [dropdown maker](https://github.com/joeyklee/itp-office-hours/tree/master/scripts/calendar-dropdown-maker) // developed rudimentary clustering algorithm for calendar suggestions

3. Wrote [some scripts](https://github.com/joeyklee/itp-resource-collector/tree/master/components/tagging-server/scripts) to get coding train videos using the youtube API & cluster them based on playlist ==> put them into the tagged resource db ==> experimented with Next.js for a [basic proof of concept](https://github.com/joeyklee/itp-resource-collector/tree/master/components/app) to generate pages from the tagged resource db

4. Updated [resource tagging browser extension](https://github.com/joeyklee/itp-resource-collector/tree/master/chrome-extension/tagging-extension) functionality and styles


***
## 20180705
***

## Meeting notes with @vanevery:
- One idea is to collect an "intro to machine learning with project X" via ML5 as a first test case to see what might be a good way to handle organizing coherent content
- We might try to come up with some small web apps that allow for the creation of organized learning pathways w/out a full blown app (e.g. dropping a json file in a web interface that produces a learning pathway and allows for commenting and editing + gets added to a searchable interface)

## Meeting with @blahah:
- Rik is working on a clever system to create and manage peer-to-peer community access to data and information
- One possibility is to use that infrastructure as a way to share, manage, and collaborate on learning pathways
- I can sketch out on paper and code what kind of UI/UX we might be interested in regarding the DIY syllabus project and do a feedback session with Rik about possibilities


## Quick update for the end of the week: 20180706

Currently working through wireframes and workflows for browsing and creating `learning pathways`, `building blocks`, and `tagged resources` in a web app/interface. Mostly right now using this as an opportunity to start thinking about information architecture and flow through the service in the case that we were to have our own homebrewed solution. Of course this is def. a heavier handed approach to this project, but I think it is a good exercise to see what an ideal case might be, so we can work towards that as a goal whether it is through smaller software interventions, etc. Still need to resolve a bunch of things, but here's just an overview image for now.

<img width="909" alt="screen shot 2018-07-06 at 19 11 57" src="https://user-images.githubusercontent.com/3622055/42403652-b21a6b52-8150-11e8-8c6f-f3b96e37af39.png">


***
## 20180626
***

**link to weekly update slides**
[https://docs.google.com/presentation/d/1iPBk2P695OF-J2qb-zQOwe796sJfpqdY39j3l4tNIJU/edit?usp=sharing](https://docs.google.com/presentation/d/1iPBk2P695OF-J2qb-zQOwe796sJfpqdY39j3l4tNIJU/edit?usp=sharing)

***

## notes
My goal this week is to spec and build out the various components to make a fully functioning prototype from end to end.

This includes:
- front end user facing interface
   + [x] TODO: create GET request to pull popular tags via API from our DB and add to browser extension for easier search and tagging (see below)
- backend user auth and resource submission database management
   + [X] TODO: create API endpoint to pull popular tags and add to browser extension for easier search and tagging (see above)
- backend database resource handling:
   + the first few tests using Github issues as our database were interesting, but I think it makes more sense now to fire up our own server/database to handle incoming data in a better/more flexible way.
   + try out firebase as a service
   + try out homegrown solution
- wiring all that up in a context that makes sense - bookmarklet? or browser extension?


## Updates

I put together a little demo to show all of the front-end mechanisms working.
![20180626-front-end-demo](https://user-images.githubusercontent.com/3622055/41928383-fbb85f50-7942-11e8-9f45-55b4b9417c8d.gif)

👉A short video can be seen here: [https://youtu.be/fWUvTobaE0k](https://youtu.be/fWUvTobaE0k) 👈

The video shows:
- grabbing title, description, and image from page meta tags
- defaults to page url if no meta tags are found
- multi select tagging with suggestions via Selectize.js
- applying level and time commitment
- submit resource button sending output data to the console

Learnings:
- need to find a good way to add titles, decriptions, and images to pages without `<meta>` tags
- still need a `rating` and `commenting` feature
- youtube has `keywords` that can be pulled from the page

A couple images:

<img width="1294" alt="screen shot 2018-06-26 at 12 53 13" src="https://user-images.githubusercontent.com/3622055/41927761-16a58a10-7941-11e8-851a-a1d5e06f9ffd.png">
<img width="1294" alt="screen shot 2018-06-26 at 12 53 55" src="https://user-images.githubusercontent.com/3622055/41927762-16b4151c-7941-11e8-91be-7a8f81f3eaeb.png">
<img width="1294" alt="screen shot 2018-06-26 at 13 02 11" src="https://user-images.githubusercontent.com/3622055/41927789-27ea94be-7941-11e8-9383-dcb028e88294.png">

# Update: 20170627

Now we've got a basic chrome extension working that sends data to a local `mongodb` instance. I still need to update the mongodb data handling in a smart way to increment the count for redundant tags and count how many times a url has been submitted etc, but the pipeline is alive and working.

TODOS:
- What's missing is authentication but I will take care of that next week.
- Also need to add the pages for the a links (e.g. `info` and `view submissions`)
- still wireframey in style so it is def. not the final design

<img width="1492" alt="screen shot 2018-06-27 at 18 35 21" src="https://user-images.githubusercontent.com/3622055/42003312-e4a1a35c-7a38-11e8-94ff-87d81402dab9.png">


## "what is the mortar to the bricks?"
I've added some ideas on this in the update slides: https://docs.google.com/presentation/d/1iPBk2P695OF-J2qb-zQOwe796sJfpqdY39j3l4tNIJU/edit?usp=sharing

It is basically what the initial proposals were. I think we're getting somewhere... still lots to be determined.

A tool link from Alejandro - "a visual tool that helps you think":
https://www.are.na/

<img width="1328" alt="screen shot 2018-06-27 at 18 46 46" src="https://user-images.githubusercontent.com/3622055/42003638-7f5dfba6-7a3a-11e8-8c86-fa44cbca8cfd.png">


***
## 20180621
***

Posting slides to: [Week 3 Updates](https://docs.google.com/presentation/d/1oHvoyg4f_30YHd53dSvAT2cjzD0RZ2EaN9PcL1zE7vk/edit?usp=sharing)

Todos:

- TF-IDF (Term Frequency – Inverse Document Frequency): https://www.youtube.com/watch?reload=9&v=RPMYV-eb6lI
   + the tricky thing about TF-IDF is that you need to have a database of text with which to compare against so that you can determine the relevancy or uniqueness of a given set of text. As an alternative, there are already a lot of smart people working on keyword and key phrase extraction, for example:
      * https://github.com/retextjs/retext-keywords
      * https://moz.com/devblog/machine-learning-approach-to-keyword-extraction/ // https://github.com/seomoz/dragnet
      * https://github.com/bxjx/gramophone
      * https://www.npmjs.com/package/keyword-extractor
      * https://www.npmjs.com/package/unfluff
- extension front-end layout and styling
- figure out suggestion for tagging mechanism (e.g. think Pocket tagging suggestions) ==> https://harvesthq.github.io/chosen/#custom-width-support ==> even better would be: https://selectize.github.io/selectize.js/

## Meeting notes with Clay Shirky


To recap our chat:
+ Shareability of feedback on resources and learning pathways should be considered as a way of being able to build better and dynamic syllabi for students
+ It is intriguing to have a kind of “slider” to filter in/out resources into a learning pathway depending on student skill level
+ There’s thinking through making and thinking before making, asking why before doing vs doing and then asking why.
+ Design for a small group, test, and see what sticks and what doesn’t - get a bunch of people for pizzas and tag resources for 2 hours and learn from that. Do this as early as possible to identify if this thing will scale. (will let you know when i’m ready!)
+ Think about community organization dynamics - e.g. TV Tropes has really amazing categorization and binning of resources under themes.
+ Think about CORAL methods - rather than choosing 1 method of knowledge acquisition that sticks with students, provide and run through as many formats

There’s probably a bunch of other ideas missing here, but those are the ones that stuck out.

Just some sketches on how to manage `user_tags` and `automated_tags` in our own database. As more users submit the same unique `url` and tag the page, we can increment the `submission_count` and append those tags under `user_tags`.

![paper sketches 68](https://user-images.githubusercontent.com/3622055/41798148-964569ca-763a-11e8-8ff2-f49384afb1af.png)


In the above image we should also add a rating/commenting reference from each user as noted in https://github.com/joeyklee/itp-diy-syllabus/issues/15



***
## 20180619
***

## Idea Sketching

Based on some of the insights drawn from the early stage prototype, I'm starting to get a better feeling  for the most realistic workflow scenarios and how we might refine the UX to reduce the barriers to submitting and tagging resources.

Just for my own documentation/stream of consciousness, I'm including some annotated sketches below.

The big takeaways from these sketches are:
1. pull out as much from the `<meta>` tags as possible
2. use the `url` as the unique identifier for the page (makes sense!) and append any duplicate submissions, tags, etc to the same resource (we might need to manage this server side)
3. send `json` and `yaml` to the issues: `json` will make it easier for us to generate a nicer wrapper around the resources and `yaml` is just more human readable.
4. make the extension more visual and take care of the states (e.g. authentication, submission)

![01-get-started](https://user-images.githubusercontent.com/3622055/41613236-11900466-73c3-11e8-8fbe-0135b247ea16.png)
![02-oauth-session](https://user-images.githubusercontent.com/3622055/41613237-11be8a20-73c3-11e8-8c70-98119863db4d.png)
![03-extension-components](https://user-images.githubusercontent.com/3622055/41613239-11fa276a-73c3-11e8-9e4c-9aadcc522671.png)
![04-submission](https://user-images.githubusercontent.com/3622055/41613240-121c093e-73c3-11e8-885a-f24d505ffdfc.png)

Now a thought is to create a list that shows all of the submitted links from a user so they might also easily find the links they've contributed.
![paper sketches 65](https://user-images.githubusercontent.com/3622055/41618409-167f20c0-73d1-11e8-85da-830e00a7a494.png)


which leads me to think, it would be also rad to have a "contributors" highlight list as incentive. Everyone wants to part of the contributors ;) + maybe even a leader board for people who've submitted the most:

![paper sketches 66](https://user-images.githubusercontent.com/3622055/41618716-f015456c-73d1-11e8-82f9-391169299143.png)

Which means we would need to ask a user if they allow / deny to be listed as a contributor:
![paper sketches 67](https://user-images.githubusercontent.com/3622055/41618830-3fd20a86-73d2-11e8-9b20-df54e4b2368d.png)

Throwing an initial set of wireframes in here:

## User clicks on extension and gets initial view
![v2-01](https://user-images.githubusercontent.com/3622055/41623965-5c80d710-73e2-11e8-92e8-f751fd7c5502.png)

## User adds tags and decides to change level and time to completion
![v2-02](https://user-images.githubusercontent.com/3622055/41623966-5c959ede-73e2-11e8-8682-4ae69a19a2d0.png)
![v2-03](https://user-images.githubusercontent.com/3622055/41623967-5ca81168-73e2-11e8-9eee-86c0cb7aabff.png)
![v2-04](https://user-images.githubusercontent.com/3622055/41623969-5cc08414-73e2-11e8-86fe-87e9b31185d4.png)

## User submits and gets delightful animation
![v2-05](https://user-images.githubusercontent.com/3622055/41623972-5cd8215a-73e2-11e8-8fd7-7548de0a645f.png)

## In Github you see the submission

Thinking out loud, but we will inevitably and most definitely get duplicate submissions. We most definitely need to think about how to manage this.

![v2-05-data-view](https://user-images.githubusercontent.com/3622055/41623970-5ccb380a-73e2-11e8-8335-27c2ce07a3a4.png)

## After submission, user gets the last view of the extension and can change the issue if necessary.
![v2-06](https://user-images.githubusercontent.com/3622055/41623973-5ce35606-73e2-11e8-8698-d450b4da4811.png)

## user clicks the `info` button on the topright.
![v2-07-info](https://user-images.githubusercontent.com/3622055/41623974-5cef724c-73e2-11e8-9805-c8dbc66f21d6.png)

## user clicks the `view all submissions` and gets all of the submissions they've made
![v2-08-all-submissions](https://user-images.githubusercontent.com/3622055/41623976-5cfc7fe6-73e2-11e8-973c-cc286ca11e57.png)

Just some notes: Linking up with @blahah from the Science Fair Project (https://github.com/codeforscience/sciencefair) - he's been working with text mining and making resources available + submission processes easier. It'll be interesting to see if there might be some good methods to intelligently extract keywords in an automated way such that we can have a baseline tagging system plus human intelligence 🤖

shiffman commented on Jun 19

This is looking great, super exciting! I love the idea of featuring contributors and even highlighting contributors, but I am a bit wary of something that "competition-driven" like a "leaderboard"?

For automated tagging something like TF-IDF might be an easy place to start just to have something simple to implement that produces results. I think I have a tutorial on that somewhere 😅


joeyklee commented on Jun 19

Hi @shiffman thanks for the feedback!

   Duly noted on the competition-driven incentives. I'm definitely much more interested to rather provide some kind of interesting feedback (e.g. a little data viz of the contributions etc)

   Yes on the TF-IDF! https://www.youtube.com/watch?v=RPMYV-eb6lI

I'll keep ya'll posted on developments :)

Thanks again!


I'm putting together some visual design propositions regardless what backend we decide to go with in the end, there will be some interface. Here's proposition A:

## Login and Auth process
![001_login-01](https://user-images.githubusercontent.com/3622055/41738222-803f6abc-755f-11e8-9a28-26c44d1f83fb.png)
***
![002_login-02](https://user-images.githubusercontent.com/3622055/41738223-8060bd84-755f-11e8-94d2-fd63eeb6b21b.png)
***
![003_login-03-auth-waiting](https://user-images.githubusercontent.com/3622055/41738224-807cfb3e-755f-11e8-8aa9-801a66128142.png)
***
![004_login-04-auth-complete](https://user-images.githubusercontent.com/3622055/41738225-808baaa8-755f-11e8-9d54-f75504c3c263.png)

## Default view, tagging and editing
![005_default](https://user-images.githubusercontent.com/3622055/41738226-80a18cb0-755f-11e8-9dea-275b747455ff.png)
***
![006_default-with-image](https://user-images.githubusercontent.com/3622055/41738227-80ad5a54-755f-11e8-96a7-94255449335e.png)
***
![007_default-submitted](https://user-images.githubusercontent.com/3622055/41738228-80c6672e-755f-11e8-85ee-83301ea3f782.png)

## Info page
![008_default-info-page](https://user-images.githubusercontent.com/3622055/41738229-80d38454-755f-11e8-9def-ec0540fab34c.png)

## user contributions
![009_default-contributions](https://user-images.githubusercontent.com/3622055/41738230-80e0c664-755f-11e8-81ec-590ba9759318.png)


joeyklee commented on Jun 22

Mm what's missing from the designs right now is a spot to put ratings and additional notes.




***
## 20180615
***

The last 2 days have been dedicated to integrating oAuth and allowing for post requests through our chrome extension. A super basic prototype is working (see images below).

Next steps:
* get renewToken working to avoid reAuth all the time
* design a UI
* refine UX
* better formatting ==> YAML is cool
* scrape page for images and include in issue for context
* scrape page for links/references ==> include them in formatted way in issue
* figure out how to deal with redundancies of issues
* write script to add coding train tagged data as initial tagged resource to test
* test across different user names

<img width="1222" alt="screen shot 2018-06-15 at 16 51 00" src="https://user-images.githubusercontent.com/3622055/41491983-36bfc7fe-70ca-11e8-99c4-88083ed1106d.png">
<img width="1222" alt="screen shot 2018-06-15 at 16 51 05" src="https://user-images.githubusercontent.com/3622055/41491984-36ed1646-70ca-11e8-92a3-3246fb5e7fda.png">
![screen shot 2018-06-15 at 16 56 40](https://user-images.githubusercontent.com/3622055/41491985-36fd4fe8-70ca-11e8-9e80-cfddae38ac5b.png)
<img width="226" alt="screen shot 2018-06-15 at 16 57 11" src="https://user-images.githubusercontent.com/3622055/41491986-37087b98-70ca-11e8-88fb-37f3517cedf6.png">
<img width="1278" alt="screen shot 2018-06-15 at 18 08 25" src="https://user-images.githubusercontent.com/3622055/41491987-3719821c-70ca-11e8-9510-e46fa4d190dd.png">
<img width="1024" alt="screen shot 2018-06-15 at 18 08 31" src="https://user-images.githubusercontent.com/3622055/41491988-3727fffe-70ca-11e8-9777-a7bb2b30bfc4.png">


 <iframe width="560" height="315" src="https://www.youtube.com/embed/hkOTAmmuv_4" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>


 Might be worth to consider crawling pages for their <meta> tag with the image

<meta property="og:image" content="https://cdn-images-1.medium.com/max/1200/1*qiqRLlNZ2b0xdlQu8qpjBQ.jpeg">


For tagging, we should have something like:

<img width="864" alt="screen shot 2018-06-19 at 10 49 45" src="https://user-images.githubusercontent.com/3622055/41605029-8de9cebc-73ae-11e8-86fc-653e5b511c9e.png">

https://semantic-ui.com/modules/dropdown.html

* allow for multiple tags to be selected or removed from a pre-canned list (e.g. pull from the existing github labels that are updated based on the submissions)
* allow for tags to be added if not in the pre-canned list

<img width="576" alt="screen shot 2018-06-19 at 10 52 24" src="https://user-images.githubusercontent.com/3622055/41605195-ea732a52-73ae-11e8-920c-556b74a39ea9.png">
<img width="638" alt="screen shot 2018-06-19 at 10 52 37" src="https://user-images.githubusercontent.com/3622055/41605196-eaa13f46-73ae-11e8-9ef0-142aeab3e1eb.png">


***
## 20180614
***

- Met with Esther and Mathura from Peblio ==> could be a front end for our app? Will whiteboard sketch ideas with them in the following weeks.
- Met with @shiffman and will check in again in the week after next ==> would be good to keep in mind untagged resources and allow people to tag and label later
   + go through workflow to determine whether to set up our own DB and then filter and manage via our own DB first then ==> send to GH issues
   + could be really good to have presets for things for "types" like videos or other pages or content
- Updates via slides here: https://docs.google.com/presentation/d/1s5cj6sMfjQ82hUabvhXYzMQOGyA1bUxj2cXIY-rdBp8/edit?usp=sharing


Note:
* June 20: Joey giving a workshop from 12:30 - 15:00 // will work from Brooklyn
* June 21: I will be part of boroughgramming w/ Brooklyn.js next Thursday June 21 // Joey will work from Brooklyn.
* June 26: Joey will brainstorm with Peblio Team w/ Esther and Mathura.


***
## 20180612
***

## Proof of concept / prototyping:
- created [itp-tagged-resources](https://github.com/joeyklee/itp-tagged-resources/issues)
   + the repo will contain the resource submissions from our contributors
   + right now contains our test submissions as we're protoyping / *pls ignore the tests*
- created [itp-resource-collector](https://github.com/joeyklee/itp-resource-collector)
   + a prototype for dealing with the authentication process into github
   + a prototype of a chrome extension / browser plug-in to link resources and text from a page and send it to our db via @mmmmmmmmmmmmmmmm .

## Next steps:
- wire up the chrome extension to our auth process // fingers crossed!



***
## 20180607
***

## Chat with Shawn

- In general, we're in sync with concept and progress
- resource tagging tool should be a priority // suggestion to perhaps start with bookmarking idea then move towards browser plugin
- definitely strong feelings for making the efforts open source, regardless if it is a workflow or software solution
- Be way of big software intervention - e.g. building rome from scratch. Think about:
   + "simplest" implementation: a shared google doc/spreadsheet between student and instructor
   + "hardest" implementation: full project management software
   + "something in between": use existing project management infrastructure/apis -- e.g. Trello API is actually pretty nice.
- keep sketching out and parsing out needs and approaches to solve/resolve challenges.


Slides for week 1 updates: https://docs.google.com/presentation/d/1hXr2e4Wup86X4Hq2g7QLGCRyHqF2oYQiBXTelpFfoBw/edit?usp=sharing


## Meeting with Dan + Dan


- @shiffman
    + linearity is really handy when going through resources (e.g. think coding train overwhelmingness)
    + ![horizontal-vs-linear-pathway](https://user-images.githubusercontent.com/3622055/41170065-e2ca4356-6b18-11e8-8d76-03027c195d9d.png)
    + if we do data management with github - e.g. using github issues as our database of resources - we need to think about:
      * how students can `make a copy` of all of the issues (tagged resources), allowing them to track their progress - e.g. by closing their own copy of the issues, pulling those issues into their learning pathways and the building blocks within those pathways.
      * a boilerplate for a class syllabus so that people aren't having to fill things in from scratch every time.
      * perhaps a front-end interface for working with the issues - how does building block & pathway creation, editing, and sharing work?
- DanO:
   + ﻿we should be as aware of possible the audience - things like github can be intimidating and unwieldy for non-developer audiences; trello is a bit more friendly - what about exploring working with their API?
   + write less software == better!
   + wary of organizing centrally around some existing platform - e.g. github or trello - working with our own DB has both advantages and disadvantages
   + making learning pathways easy on the eyes == a nice feature for our audience (similar to shiffman's remarks)
   + ![vertical-pathway-good](https://user-images.githubusercontent.com/3622055/41170438-5b528152-6b1a-11e8-9f56-f016cc99a428.png)




## Next steps

- Bottom up learning pathway creation
      + try to create a couple learning pathways starting with a bunch of resources to get to an end goal (e.g. fundamentals of javascript)
- Top down learning pathway creation
      + try to create a couple learning pathway starting with a completed project and break down the steps
- Get access via Yen to the syllabi and people database

##  refs:
   + https://www.imsglobal.org/activity/learning-tools-interoperability


***
## 20180603
***

* Nice to haves/ideas:
   - document issues: make sure students and GRAs can provide feedback about what worked/didn't work in the learning pathway
   - how to document a project:
     + template for case studies ==> need header image, descriptions, links == >everything must be filled out before submission
     + it's like Wiki  // look into wiki's structure wise
     + people should enjoy the documentation process and the referencing process
      + export function for documentation (press kit style, ready to use material for documentation)
   - super important: develop a system for concepting
     + getting to the right concept as a crucial step ==> e.g. what are the references and projects which have happened in the past / past projects / past designers/ artists
     + tag past projects, tag books, papers, articles, links, inspiration

- "related projects" suggestions list based on tech or methods or links used or referenced ==> bring you forward towards new or mashuped methods, etc
- add emotion tags ==> eg. happiness, relief, frustration
- add a "slider" for range of "prototype, proof of concept ==> production"
- create level of difficulty tags?

What is the design system for solving the curation of materials for individualized learning, discovery, etc ?

Ways of working ==> include more philosophical styles of doing // e.g. design sprints or 2-2-2 (or whatever it is called), iterations, ...

We are building a platform to:
- do better problem solving
- curate the management of projects
- better reference the problem solving process
- break down complexity
- find the right steps/methods/tools to turn your idea into reality
- build off of the materials of others and make references to them
- ...



***
## 20180601
***

Meeting notes

Started briefing for DIY Syllabus: https://docs.google.com/document/d/14wtkBoX1fbWLUpeSw2PBLTRhv4-qsjQtfIXQNBGMFLE/edit?usp=sharing
Started moodboard for DIY Syllabus: https://docs.google.com/presentation/d/1aA80h4-t3FuK8H1JkA_M12orFMegoaA-c_IxaWGZGEs/edit?usp=sharing


## Additional Ideas:
* ITP camp as a test case
* Clay Shirkey - ed tech / https://www.nyu.edu/about/leadership-university-administration/office-of-the-president/office-of-the-provost/academic-affairs/clay-shirky.html

# Todos/handy tools for concept:
* [X] "User" personas ==> see: https://github.com/joeyklee/itp-diy-syllabus/blob/master/docs/concept/personas/PERSONAS.md
* Journey maps
* service blueprints
* feature blueprint
* MVP vs. dream project specs


***
## 20180430
***

# 20130523

## Recap from last conversation

To briefly recap our conversation:

- ITP is looking for an educational technologist type-of-person to design, develop, and test various types of software and community based interventions that will help build greater access to course materials, student work, and infrastructure internally and externally.
- Specific efforts include:
    + designing methods for gathering metrics about the department IMA support
    + highlighting student work (e.g. blog blender)
    + providing community support for portfolio feedback
    + gathering and archiving course materials
    + enhancing equipment rental processes and room booking at the BK location
    + enhanced course planning and projections for students
    + p5 / p4 web editor integrations
    + easier attendance monitoring




***
## 20180523
***

# meeting notes 20180525

The tasks cover 3 main target areas / main stakeholders:

* specific classes -- professor/student
* admin & data // efficiency internally -- admin/students
* future courses  -- students

## Ideas for focused work for 3 months

* Just-in-time/DIY syllabus:
  - start with the CODE! class as a test ground
  - bring in syllabi from other courses and other online tutorials and materials
  - syllabi currently live across the web in the form of:
     + "Classes" LMI
     + Github
     + html
     + WordPress
     + GoogleSites
     + PDFs

* IMA is starting and they need a portfolio / way to highlight student work / the project "blender" where students and people can share, comment, and see what's happening at ITP/IMA + a way to archive.

* One way to better manage data would be to develop some system to better tag and keep track of links across all the sources of materials and content across the department and students. Thinking about a way of better indexing, searching, ontologically tagging links ==> see https://pinboard.in/


# Next steps

* take care of admin details
* collaborate with Markus Kreutzer for concept, design, and implementation (http://markuskreutzer.com/) - based in germany + will subcontract to do the projects together.
