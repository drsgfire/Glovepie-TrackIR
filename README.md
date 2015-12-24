# Glovepie-TrackIR
Some scripting to help you get started in assigning different functions to TrackIR axis.

The primary reason for creating this comes from a need to lean. Fairly simple in simulation games like ARMA and flight simulators but doing this function in FPS is another story. Keybinds and buttons are your only option so we needed a way to convert TrackIR axis input to a keybind to set to lean function.

I'm not really a coder by nature but I saw a need, did a little reading and now I have a working script for TrackIR. This can now be used by any game that has a lean function. Just edit the script to use the keys you would like and then bind it in game.

The TrackIR script includes a numerical value that corrisponds to the TrackIR's ingame axis value.

TrackIR's curves are measured in:
THA (True Head Angle in Degrees)
GHA (Game Head Angle in Degrees)
RS  (Rotation Speed)

This is basically where things get tricky and is why I am putting this script on github. I have played around with a custom profile in TrackIR's profiler to have no input on the X, Y, Z, pitch and yaw axis.

TrackIR has an 11 point adjustable curve for each axis. By default this curve is set to mirror center which will give you the same input curve opossite of each other.

Testing has been done with the following curve on the Roll axis:
Point 1 (Center) X=0 Y=0
Point 2 X=2.9 Y=20
Point 3 X=3 Y=20
Point 4 X=3 Y=20
Point 5 X=3 Y=20
Point 6 X=3 Y=20
