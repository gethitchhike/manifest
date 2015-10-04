![alt tag](https://avatars0.githubusercontent.com/u/13689977?v=3&s=200)
#Hitchhike manifest

This manifest describes the targets behind the project and should help to keep them observed.

##Satisfy the KISS principle

The first target is to satisfy the KISS principle to keep the system as simple as possible.

You often have many functions you use only once a year. That's not enough to implement them in this project.

Every function is as simple as possible designed to just reach the main objectives. No more, no less.

I call it "advanced KISS principle" because an important point is that the system should bring the most needed components, too.
Most of the users shouldn't go without the functions they need for regular usage. But anything you don't need very often won't be part of this system.

##Everything is a plugin

The system itself doesn't know at the point of programming which plugins are used. 
Everything (except the boilerplate) will be bootstrapped dynamically. 
Any function in the system is a plugin. Also plugins can have depencies to other plugins.

###Keep 3rd party dependencies flat

Sometimes you need to use 3rd party libraries to get your plugin working. Sure, you can do that. But keep it flat. And throw them in `/Lib/`

###Only create config values if you need to

Config handling is difficult (at M1). You should only create new ones if you really need to.

##CDN

Frontend and backend templates shouldn't contain CDN references. 
CDNs are cool, but if you don't have a working connection and/ or it's blocked or don't want to connect to them, they are useless.

##Privacy

The system will have statistic modules, too. But the goal of statistics isn't to track individual users. 
The statistics should only show how many views you get. And that's all!

Have fun.
