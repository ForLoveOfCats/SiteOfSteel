
# New Player Model for 0.1.4
<sup>Posted 7/21/19 by ForLoveOfCats</sup>

<br>

Apologies for the past few weeks, I was unable to work for a for a
while for personal reasons and then had to leave on a trip (with
another trip in a few weeks). However I've made notable progress this
week so lets get right into it!


<br>
<br>
<br>


## SkyOfSteel mentioned in latest Godot devblog
Thats right! The latest post on the Godot blog features SkyOfSteel
front and center! You can go give it a read
[here](https://godotengine.org/article/csharp-android-support).


<br>
<br>
<br>


## SkyOfSteel has surpassed one thousand commits and one hundred downloads!
<br>

![Image of one thousand commits](NewPlayerModel/OneThousandCommits.png)

<br>

![Image of one hundred downloads](NewPlayerModel/OneHundredDownloads.png)

<br>

If you enjoy SkyOfSteel please consider rating it on
[Itch](https://forloveofcats.itch.io/skyofsteel), giving it a review,
and sharing it with your friends! The best way for any indie game to
grow is through word of mouth so any help on that from is greatly
appreciated!


<br>
<br>
<br>



## New player model
I've been working on this for a few weeks but the new model is now
in-game and playable.

<br>

![Picture of new player model](NewPlayerModel/3rdPersonModel.png)

<br>

The texturing is almost non-existant and the eyes are *going* to
change. Over the next week I plan on animating the head and legs to
show the player's up/down look angle and their forward/backward
movement input respectively.


<br>
<br>
<br>


## Rocket jumping improvements
I've improved the functionality and feel of rocket jumping
conciderably. Previously the rocket would pass through the surface it
hit before exploding. Because of this it was not as reliable as I
would have liked and in addition prevented me from adding a check to
prevent pushing items and players through surfaces. I've fixed this
with some odd raycast abuse so now the rockets actually hit where they
are supposed to and we now check for surfaces between the rocket and
anything it tries to push.

Also contributing to the improved feel is the fact that rockets now
come out of the center of the player. This is important as the center
is also the reference location for calculating the push applied to the
player when a rocket explodes.


<br>
<br>
<br>


## Added ground pound
*This one may be subject to removal*

Now when pressing crouch in the air, a player will start immediately
decending (without affecting horizontal momentum). This new feature is
highly WIP and explorative.


<br>
<br>
<br>



## The player is now 50% larger
This is for the FPS combat coming soon as it allows the player to
provide a better target for shooting.


<br>
<br>
<br>


## Added a generic cooldown
Now when switching inventory slots, placing tiles, removing tiles,
dropping/picking up items, firing the rocket jumper, ect, there is a
cooldown before you can use the selected item. In some cases (such as
firing the rocket jumper) this also prevents switching slots until the
cooldown has finished.

<br>

<video width="80%" controls>
<source src="NewPlayerModel/Cooldown.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>


<br>
<br>
<br>


## Refactored build system and general item information lookup
It is now much simpler and less brittle to add new items to the
game. While we are not there yet, this is yet another step toward
allowing mods to create custom items and tiles. An awesome side effect
is that this make it very easy to fix a little bug allowing walls and
triangle walls to be placed intersecting. This has been fixed.

<br>

![Picture of a wall blocking a triangle wall](NewPlayerModel/WallInWall.png)


<br>
<br>
<br>


## Added World.DebugPlot

<br>

![Picture of many plot points on a wall and floor](NewPlayerModel/DebugPlot.png)

<br>

This is a simple way to visual 3d positions when debugging. It proved
invaliable when redesigning the rocket collision.


<br>
<br>
<br>


## Focuses for finishing up 0.1.4
Over the next week I intend to wrap up the new player model with more
texture work as well as adding head and leg movement before adding in
the first hitscan firearm! That's right, a major forcus of next week
is to get FPS combat implimented. 0.1.4 is shaping up to be a great
release ;)


<br>
<br>
<br>


## And now a message from our sponsor, YOU!
SkyOfSteel is, and always will be, free. However if you enjoy
SkyOfSteel and value my work, any support on
[Patreon](https://www.patreon.com/user?u=19556107) is greatly
appreciated. If you cannot help to support me financially or do not
wish to, thank you anyway for your support and interest!


<br>
<br>
<br>


# Remember to rate on Itch, share with your friends, and until next time, Cheers!

<br>

<iframe src="https://itch.io/embed/372880?linkback=true&amp;border_width=5&amp;bg_color=77b0ff&amp;fg_color=000000&amp;link_color=14e500&amp;border_color=4c4c56"
			  width="800" height="175" frameborder="0"></iframe>

<br>
<br>
<br>
<br>
<br>
