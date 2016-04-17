---
layout:     post
title:      fsm_docker
date:       2015-09-01
summary:    a finite state machine orchestration framework for your docker containers
permalink:  /:title
---

#### Construction in progress
* * *

So I have used `docker-compose` and seen how that is abstracting containers as *services*. But that does not seem to have a finer control on when those services start / stop / execute something based on the state of other services *(from my current knowledge on it)*.

I think a finite state machine for the entire setup where each state directs a service to do some action and moves to another state based on the next input from outside - say a `docker-compose.yml`-ish file will

* Have resilience on states of services and a way to retract if faced with errors
* Dynamically change state of the services when a trigger it presented. For eg. when a log entry is generated, run a script on a contain for it to map / save it
* Many more which I have not yet explored on.

* * *
So if you are out there reading this rant, Check out this [Github repo](https://github.com/lookageek/fsm_docker) leave an issue there if you have more ideas and / or want to collaborate. Or shoot me a DM on twitter *@manklu*
