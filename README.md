# Xbox Gamepad/Controller Input with Jinput

This is an example of how i managed to use the Jinput-library to get input-signals from an Xbox360-Controller. I wanted to get just a single impulse, if i trigger a button/stick, what is working for me so far. It may not be the best solution, but i wanted to share it, if somebody else has problems getting started with Jinput.

I was only able to test this under Windows 10 with an Xbox360-Controller (wired). It should be working under Linux and MacOS too, but i can't say anything about the compatibility with other controllers.

*Note: There are probably some issues, if both analog-sticks are used at the same time.*

# Getting started

You need to import Jinput to your project. I've used [Jinput 2.0.6](http://mvnrepository.com/artifact/net.java.jinput/jinput/2.0.6) but you can also use the [latest build](http://ci.newdawnsoftware.com/job/JInput-git/), if you need something like the Windows 8/10-warning gone.

The next thing you need are the native libraries of Jinput. You get these here:

* [Windows](http://repo1.maven.org/maven2/net/java/jinput/jinput-platform/2.0.6/jinput-platform-2.0.6-natives-windows.jar)
* [Linux](http://repo1.maven.org/maven2/net/java/jinput/jinput-platform/2.0.6/jinput-platform-2.0.6-natives-linux.jar)
* [MacOS](http://repo1.maven.org/maven2/net/java/jinput/jinput-platform/2.0.6/jinput-platform-2.0.6-natives-osx.jar)

Create a folder in your project for the native libraries and unpack the .JAR-File(s) in this folder.

Make sure to add `-Djava.library.path=pathname` in your projects VM Options.

