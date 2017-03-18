# NoSight
Putting tape over your webcam won't help you but this will.

So in 2014 I made this applescript to automate turning off and on my iSight camera on my MacBook Pro.  It should work on any Mac.  Basically what it does is deny read access to the "QuickTimeUSBVDCDigitizer" plugin located at "/System/Library/QuickTime/QuickTimeUSBVDCDigitizer.component/Contents/MacOS"  and also denies "VDC" from being read which is inside of "VDC.plugin" located at "/System/Library/Frameworks/CoreMediaIO.framework/Versions/A/Resources/VDC.plugin/Contents/MacOS/"

If you open the Applescript file inside the script editor part of MacOS you'll see in detail every step that is made including "/bin/chmod a-r" argument that is the secret sauce.

Applescript is a very powerfull scripting language that can even make system calls with Unix commands.  I went ahead and made this script into an application to made it kinda of pretty.  You can toggle between and off and on state.  Keep in mind that this doesn't just disable a built-in camera.  It will turn off video input for all sources connected to your Mac.

The video input will really be off and NO you can't bypass this.  So the old trick of having the camera on but disabling the green indicator light isn't going to fool this.  This is as good as cutting off the power from the computer.  You know that saying about the only secure computer is the one that's turned off and sunk at the bottom of the ocean?
