# Actor Framework

Predigame Actors are Sprites that perform certain **actions** - mostly in the form of animations that make the game more realistic. Actors can perform any number of actions (walk, run, jump, attack) which are usually left up to the artist's creation of the sprite.

Here are a few example Actors:

![alt text](http://predicate.us/predigame/images/zombie_animated.gif "Predigame Zombies")

![alt text](http://predicate.us/predigame/images/other_animated.gif "Predigame Actors")


## Asset Licenses

All static artwork has been obtained from  [OpenGameArt](https://opengameart.org/)  or from Google with the "Labeled for reuse" filtered defined. Animated sprites are licensed to Predicate Academy (Predigame's developer) for use limited to non-commercial Predigame development.


## Prerequisites
You'll need to have the Predigame platform installed, a trusty text editor handy, and the command prompt (or terminal) open to complete this tutorial. Visit [http://predigame.io](http://predigame.io) for installation instructions.

## Getting Started
To get things started, we're going download an existing Predigame game that has a few actors we can use to experiment with animations (you'll need an Internet connection to complete the download). This can be done by typing the following the command in the terminal:

```
pred pull actors
```

Then change into the `actors` directory.

```
cd actors
```

## How Actors Work
The artwork we use for actors are called *four directional sprites* in that each of the actions are repeated in each direction of movement (up, down, left, right). Actor animations may seem a bit complicated under the hood, but it is nothing more than just a sequence of still images that are refreshed at a fast enough rate to give the **illusion of animation**.

In Predigame we store actors as **.pga** files in the `actors` directory. Every **.pga** file of actions and directions as highlighted in the picture below:
![alt text](http://predicate.us/predigame/images/actors.png "Predigame Actors ")

Each of the highlighted png files capture a single frame.
![alt text](http://predicate.us/predigame/images/actors2.png "Predigame Actors ")

And when those frames are rotated fast enough the actor (in this case the zombie) appears to be attacking! Pretty cool, right?

Now let's explore some animations. We provided a simple animation utility that enumerates through all possible animations for a given actor (just hit the space bar). Want to speed up or slow down the animation? Try using the `-` and `=` keys.

Here's a few examples for running this utility:

```
pred animation.py Bee
pred animation.py Skeleton
pred animation.py Soldier-1
pred animation.py Viking
pred animation.py Witch
pred animation.py Zombie-1
```

## Next Steps

Want to see actors in action? Take a look at the [Making Bacon](/examples/bacon) game.
