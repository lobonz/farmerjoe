## Farmerjoe - The Render Farmer

#### NOTE: FARMERJOE 0.13 DOES NOT WORK WITH BLENDER 2.5 ONWARDS

Farmerjoe is a distributed rendering system for Blender, it does both frame based distribution and bucket based (single frame) distribution, it has a web gui and is fairly easy to set up IMHO :) I had tried to get Drqueue running and it worked great on linux but was less than easy to use on windows. There are a few other distributed rendering systems for blender but I wanted something I could run independantly of blender and seeing how I knew perl I hacked together this system to get distributed rendering running for Blender the way I wanted it to work.

### Why Another Network Rendering System?

I originally tried to get DrQueue working, and while a very good system is a bit of a mission to get installed for windows and after struggling with it I figured that rather wasting anymore time trying out other systems, I would just write one that did things the way I wanted.

### How is Farmerjoe Different?

Well, I hate having to install all sorts of stuff to get another render slave working so Farmerjoe is designed to have no install for render slaves. I also dont like having to install much for the server, and as I only really know how to program in perl I wrote the whole system in Perl as a (single script for the mostpart) and also compiled it to an exe version so you dont even have to install perl. Farmerjoe also is, I think one of the first distributed rendering systems for Blender to do both frame based and bucket rendering. (bucket rendering = rendering a single image in parts afaik)

### What Platforms does Farmerjoe Work On?

In theory any platform blender and perl and blender run on, but I have only run it on Linux, Windows and now OSX, to run on other platforms a bit of code would need changing, I can fo this but cannot compile it as I only have Lin/Win/OSX

There are Windows, Linux and OSX Binaries included.

The binaries were made using PAR a free perl module which packs perl code into a single executable binary.

### Web App UI
![](https://github.com/lobonz/farmerjoe/blob/master/preblender2.5/web_ui.png?raw=true)

### Blender Python UI
![](https://github.com/lobonz/farmerjoe/blob/master/preblender2.5/bpy_ui.png?raw=true)
