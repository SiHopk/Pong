# Pong
A simple Pong game made inside of GameMaker Studio 2. This game was made as a first project for a college class in the span of a few days. This game is made up of 8 objects total, each with its own set of events coded to tell each object how to act once the game ha begun, and the user has started to interact with it. The most important of the eight objects being the player paddle, the enemy, the ball, and the two goals that will keep score for the player and enemy. 

## Objects
Below will be listed each object, as well as a table containing each of its events and a description of what each event does.

### Paddle
This object is the players paddle, its job is just to move up and down only when the player gives the input to do so.

|Event|Description|
|-------|------------|
|Key Down - No Key|This event makes the paddle stop moving if there is no user input|
|Key Down - Up|This event tells the paddle to move upwards when the user presses the up key|
|Key Down - Down|This event tells the paddle to move downwards when the user presses the down key|

### Enemy
This is the enemy paddle it will simply follow the ball on the y axis.

| Event | Description |
|-------|-------|
| Step | This event says that for evey frame the ball exists, this paddle will follow along the y axis |

### Goal1
This object keeps score for the enemy paddle

| Event | Description |
|-------|-------|
| Creation | This event will initialize the enemy score to be 0 |
| Draw | This event tells the object to draw its own sprite, so that is doesnt dissapear, as well as the enemys score on the board|
| Ball Collision | This event tells the goal that when the ball collides with the goal it increases the enemy score |

### Goal2
This object keeps score for the players paddle

| Event | Description |
|-------|-------|
| Creation | This event will initialize the players score to be 0 |
| Draw | This event tells the object to draw its own sprite, so that is doesnt dissapear, as well as the players score on the board|
| Ball Collision | This event tells the goal that when the ball collides with the goal it increases the players score |

### Announcer
This is an invisible object that greets the player once the game is booted up

|Event|Description|
|-------|-------|
|Game Start|This event has the announcer greet and instruct the player on how they can reset the vall should they have any sort of issues with the ball|

### Ball
This is the ball that bounces around the field

| Event | Description |
|-------|-------|
| Key Pressed - Space | This event will reset the ball shoud it get stuck on anything |
| Barrier Collision | This event tells the ball to bounce off the barriers and plays a sound for the collision |
| Enemy Collision | This event tells the ball to bounce off enemy paddle and plays a sound for the collision |
| Paddle Collision | This event tells the ball to bounce off the players paddle and plays a sound for the collision |
| Goal1 Collision | This event tells the ball to reset its position and play the sound for scoring a goal |
| Goal2 Collision | This event tells the ball to reset its position and play the sound for scoring a goal  |
| Game Start | This event tells the ball once the game starts where to spawn, then has it randomly choose a direction, and finally tells it how fast to go in that direction |

### Room0
This is the level the game will be taking place inside of.

|Event|Description|
|-------|-------|
| Creation Code | This event simply tells the room that if the music for the game is not playing, then it should play the music on a loop for the player|

### Barrier
Bounces the ball off of them, this object has no events

### MiddleLine
This is a decorative object and as such it has no code.
