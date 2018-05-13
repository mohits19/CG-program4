# Computer Graphics (CSC 561)
### Program 4: Missile Command
This is a version of the classic Atari game, Mission Command. The objective of the player is to protect 6 cities against descending missiles by firing anti-ballistic missiles at them. The game ends when all cities and batteries are destroyed!! The player gets 10 points for a missile and 100 points for a spaceship. 

This game was programmed with the help of **three.js** library.

#### _Part 1_ (Display the field and sky)
The basic models required for the game were rendered; Terrain (a simple plane), 6 Cities (cuboids) and 3 Missile batteries (cones). All the models rendered are 3-Dimensional.

#### _Part 2_ (Display and animate descending missiles)
After every fixed period of time, a missile (red cones) is created. Each missile originates at a random position at the top of the screen and moves towards a randomly selected target (any of the not-yet-destroyed 6 cities or 3 missile batteries).

The interval between each missile launch and speed of missiles can be changed to make game easier or harder as required.

#### _Part 3_ (Display and animate ascending missiles)
On a mouse click, an anti-ballistic missile (yellow cones) is created. They originate from the closest not-yet-destroyed battery and move towards the point of mouse-click.

#### _Part 4_ (Add interaction with descending missiles)
When a missile intersects a target (city or battery), they are both destroyed. Similarly, when an anti-ballistic missile intersects with a missile, they are both destroyed.

When all the 9 targets have been destroyed, the game ends!

#### _Extra Credits_
1. **Split descending missiles every so often** - every so often, a missile is cloned and sent towards a different target.
2. **Animate missile-missile and missile-city/battery explosions** - when a missile-missile or a missile-city/battery intersection happens, in addition to removing both objects from scene an explosion object is added.
3. **Add periodic spaceships flying through as unusual targets players can shoot** - every so often, a spaceship moves across the screen horizontally which can be destroyed using an anti-ballistic missile.
3. **Track and display score** - Score is displayed on the top left corner of the screen. Every missile hit is worth 10 points and every spaceship is worth 100 points.
4. **Sound and music** - On events like game start, missile launch and explosions, the corresponding sound effects are played.
