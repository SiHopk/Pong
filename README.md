# Pong
A simple Pong game made inside of GameMaker Studio 2. This game was made as a first project for a college class in the span of a few days. This game is made up of 8 objects total, each with its own set of events coded to tell each object how to act once the game ha begun, and the user has started to interact with it.

## Objects
Below will be listed each object, as well as a table containing each of its events and a description of what each event does.

### Paddle
This object is the players paddle, its job is just to move up and down only when the player gives the input to do so.

| Event | Description|
|-------|------------|
| Key Down - No Key| This event makes the paddle stop moving if there is no user input|
| Key Down - Up | This event tells the paddle to move upwards when the user presses the up key |
| Key Down - Down| This event tells the paddle to move downwards when the user presses the down key |

### Enemy
This is the enemy paddle it will simply follow the ball on the y axis.

| Event | Description |
|-------|-------|
| Step | This event says that for evey frame the ball exists, this paddle will follow along the y axis |

### Goal1
This object keeps score for the enemy paddle

| Event | Description |
|-------|-------|
| Creation | Initializes the enemy score|
| Draw | Tells the object to draw its own sprite as well as the enemys score on the board|
| Ball Collision | When the ball collides with the goal it increases the enemy score |

### Goal2
This object keeps score for the players paddle

| Event | Description |
|-------|-------|
| Creation | Initializes the players score|
| Draw | Tells the object to draw its own sprite as well as the players score on the board|
| Ball Collision | When the ball collides with the goal it increases the players score |

### Ball
This is the ball that bounces around the field

| Event | Description |


### Barrier
Bounces the ball off of them, this object has no events


