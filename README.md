# Xbox Gamepad/Controller Input

This is an example of how i managed to use the Jinput-library to get input-signals from an Xbox360-Controller. I wanted to get just a single impulse, if i trigger a button/stick, which is working for me so far. It may not be the best solution, but it's working for me and i wanted to share my solution, if anyone else has problems getting started with Jinput like myself.

I was only able to test this under Windows 10 with an Xbox360-Controller (wired). It should be working under Linux and MacOS, but i can't say anything about the compatibility with other controllers.

*Note: There are probably some issues, if both analog-sticks are used at the same time.*

# Getting started

You need to import Jinput to your project. I've used [Jinput 2.0.6](http://mvnrepository.com/artifact/net.java.jinput/jinput/2.0.6) but you can also use the [latest build](http://ci.newdawnsoftware.com/job/JInput-git/), if you need something like the Windows 8/10-warning gone.

