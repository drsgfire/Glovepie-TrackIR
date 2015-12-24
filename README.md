# Glovepie-TrackIR
Some scripting to help you get started in assigning different functions to TrackIR axis.

The primary reason for creating this comes from a need to lean. Fairly simple in
simulation games like ARMA and flight simulators but doing this function in FPS is
another story. Keybinds and buttons are your only option so we needed a way to
convert TrackIR axis input to a keybind to set to lean function.

I'm not really a coder by nature but I saw a need, did a little reading and now I have
a working script for TrackIR. This can now be used by any game that has a lean
function. Just edit the script to use the keys you would like and then bind it in game.

The TrackIR script includes a numerical value that corresponds to the TrackIR's
in-game axis value.

TrackIR's curves are measured in:
THA (True Head Angle in Degrees)
GHA (Game Head Angle in Degrees)
RS  (Rotation Speed)

These values are plotted on the curve chart by X and Y.

This is basically where things get tricky and is why I am putting this script on github.
I have played around with a custom profile in TrackIR's profiler to have no input on
the X, Y, Z, pitch and yaw axis.

TrackIR has an 11 point adjustable curve for each axis. By default this curve is set
to mirror center which will give you the same input curve opposite of each other.

Testing has been done with the following curve on the Roll axis:
Point 1 (Center) X=0 Y=0
Point 2 X=2.9 Y=20
Point 3 X=3 Y=20
Point 4 X=3 Y=20
Point 5 X=3 Y=20
Point 6 X=3 Y=20

This has been tested in Rainbow Six Siege and works pretty well. One thing I have
thought about changing though is to use the X axis instead of the roll axis.
I noticed after a short amount of time, my neck was starting to ache a bit. The roll
amount really is not that much but the fact that you have to put some conscious
effort into moving back to a general centered position causes some strain. On the
X axis you would be keeping your head straight and just shifting your body to the left
or right which would shift your head left and right of center. I have not tested this but
naturally it tends to feel better on your neck. Also you would not get random noise as
bad from using the X axis. What is meant by this is getting a different axis input
when you only intend it to come from one input.

An example would be yawing your head to look left and right. Even though you only
want the roll axis to be your input, just the action of moving your head left and right
cause some form of roll input. Shifting on the X axis should get rid of this problem.