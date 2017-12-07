A mod for the OpenRA rts engine that adds time travel as a game mechanic.

The idea for time travel was inspired by the old Red Alert games, Whos story is built around it. Unfortunately the chronosphere was restricted to teleportation. I didn't come back to it until I encountered another RTS called Achron and was disapointed that it was no longer an active game. Once Achron closed its multiplayer servers there was once again no RTS with my favorite game mechanic. So I'm setting out here to create one. 

I'll have to save the game state somehow at each tick. 
However this will take up a lot of memory real fast. So i'm going to do some kind of compression. I'm thinking about keyframes and tweens as a way to compress some types of actions as linear equations and make the state retrievable for render in O(sqrt(n))

This means i'll have to rework exactly how every value pertaining to Actors change over time.
This may be as simple as implenting custom traits.



To Install first download and install OpenRA.
Then copy and paste the 'timetravel' folder to /path/to/OpenRA/mods

Released under the GNU general public license.
