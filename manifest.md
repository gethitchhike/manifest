![alt tag](https://avatars0.githubusercontent.com/u/13689977?v=3&s=200)
#Hitchhike manifest

This manifest describes the targets behind the project and should help to keep them observed.

##Satisfy KISS-Principle

The first target is to satisfy the KISS-Principle to keep the system simple as possible.

Often you have dozen of functions you use once a year. That is not enough to implement them in the project.

Every function is simple as possible to allow the reach the main goal, without bells and whistles.

I call it "advanced KISS-Principle", because a important point is that the system should bring the most needed components, too.
Most of the users should not go without the functions they need for regular usage, but anything you don't need enought, will not be part of the system.

##Everything is a plugin

The system itself does not know at the point of programming which plugins are used. 
Everything (except the boilerplate) will be bootstrapped dynamically. 
Any function in the system is a plugin. Certainly, the plugin can have depencies to ofter plugins which are needed to get fulfilled.

###Keep 3rd party depencies flat

Sometimes, you need to use 3rd party libraries to get your plugin working. Sure, you can do that. But keep it flat. And throw them in /Lib/

###Only create config values if you need to

Config handling is difficult (at M1), you should only create new ones if you really need to.

##CDN

Front- and backend templates should not contain CDN's. 
CDN's are cool, but if you don't have a working connection and/ or its blocked or you don't want to connect to them, they are useless.

##Privacy

The system will have statistics-modules, too. But the goal of statistics is not to track the user. 
The statistics only should show how many views you get. Nothing more.

Have fun.
