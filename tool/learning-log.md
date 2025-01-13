# Tool Learning Log

## Tool: **p5play**

## Project: **Soccer Game**

---

### 9/30/24:
* [p5play:Learn](https://p5play.org/learn/index.html)
* [p5play-Docs](https://p5play.org/docs/index.html)
* [p5.js Reference](https://p5js.org/reference/)

### 10/20/24:
* [p5play: Sprites](https://p5play.org/learn/sprite.html)
  * [Basic Properties](https://p5play.org/learn/sprite.html?page=0)
    * Read through the examples
    * Changed values of `sprite.basic-property = value` which changed things like x/y position, width, height, color, diameter, rotation, and text-size.
    * Did level 0 challenge which asked to create a blue circle and place it in the top right corner of the canvas
  * [Physics](https://p5play.org/learn/sprite.html?page=1)
    * Learned about `.collider` which detecs collisions of a sprite with other sprites.
    * `.collider` types are `s`(static), `k`(kinematic), `n`(none), and the default `d`(dynamic)
    * also learned about `world.gravity`
  * [Movement](https://p5play.org/learn/sprite.html?page=3)
    * learned about different movements and properties that affect/cause the movement
    * `velocity`, `direction`, `speed`, `move`, `moveTo`, `moveTowards`
  * Continued through the rest of the lessons on `Sprites` and changed lines of code to see what it did and what it changed in the example and challenges.
* I went through the [Group](https://p5play.org/learn/group.html), [Animation](https://p5play.org/learn/animation.html), [Input](https://p5play.org/learn/input.html), [Camera](https://p5play.org/learn/camera.html), [Joints](https://p5play.org/learn/joints.html), [Canvas](https://p5play.org/learn/canvas.html), and [World](https://p5play.org/learn/world.html) sections.
* I plan on making a mini project using the properties I learned and watch videos on p5play.

### 10/27/24:
* Watched these three videos on p5play
  * [Basics](https://www.youtube.com/watch?v=5addy2G5DIc&list=PLoHS9P-kC-252Pd9MJD_ItfaVuYV2kTCE&index=1)
  * [Physics](https://www.youtube.com/watch?v=cPTrLLdCX-Y&list=PLoHS9P-kC-252Pd9MJD_ItfaVuYV2kTCE&index=2)
  * [Movement](https://www.youtube.com/watch?v=p0vk5HlcFA8&list=PLoHS9P-kC-252Pd9MJD_ItfaVuYV2kTCE&index=3)
  * Helped me review the things I learned in the docs of p5play and get a better understanding of what I need to have in order to make p5play run in my own website.
* [This](https://jsbin.com/qudinafaso/edit?js,output) is my mini project.
  * It is pretty simple
  * Includes things like `collision`, `color`, `stroke`, `velocity`, and `kb.pressing`.
* I plan on making this project a little more advanced or make a new project and include different properties.

### 11/4/24:
* I worked on adding more elements to my mini project on [here](https://jsbin.com/nayekaheyu/edit?js,output).
  * I added a little "goal-like" area
  * Made the canvas bigger
  * Added a new block/player
  * I need to try to fix the movement when pressing a key (so it only moves 1 player instead of both)

### 11/11/24:
* [Input: Keyboard](https://p5play.org/learn/input.html?page=1)
  * helped me fix the movement mistake in my project
  * needed to add 'arrow' to the direction of the `keyboard.pressing` function so it only moves player 2
* I made a [new project](https://jsbin.com/genizumemi/edit?js,output)
  * used starter code from [here](https://p5play.org/learn/sprite.html?page=10)
  * added `kb.pressing` functions that affected `vel.x` (`arrowLeft` --> move left, `arrowRight` --> move right, `space` --> move up/fly)
  * added a function for when the drone is `colliding` with the floor which doesn't let it move left/right
  * I plan on working on this project more

### 11/18/24
* I continued working on the [project](https://jsbin.com/sutogidufe/edit?js,output)
  * added more `if` statements to change the `collider` of the drone and used `kb.presses` to do so

### 11/24/24
* Revisited the [World](https://p5play.org/learn/world.html) and [Joints](https://p5play.org/learn/joints.html) lessons
  * helped me understand the `.sleeping` which means the sprite isn't moving or colliding with anything new
* used the starter code of the 'gluejoint' and 'sleeping' examples in my new [project](https://jsbin.com/matirileci/edit?js,output)
  * changed the canvas size
  * changed the starting positions of the sprites
  * added a new sprite called 'brick'
  * added `if` statements
    * to prevent the ball from flying out of the canvas (if ball = 0 or 1000, it will bounce back at a `velocity` of 5)
    * to see if ball is `colliding` with the brick, `ball.sleeping` would be set to `false` and the brick would `rotate` to make the ball fall then return to normal state

### 12/8/24
* Watched [this](https://www.youtube.com/watch?v=5jjnVeZCSwM) video
  * Went over sprites and the values you can include in it
  * Sprite(x, y, width, height or 'shape')
  * If you only define 'width' you get a circle
  * Both 'width' and 'height' --> square/rectangle
  * var_name = Sprite(x, y, width, height or 'shape') to later add properties (var_name.property = __)
* Worked on [this](https://jsbin.com/gihekoxiyu/edit?js,output) new project
  * Used starter code from [here](https://p5play.org/learn/tiles.html)
  * Added more 'tiles' and 'spaces' to make '.PLAY"
  * Learned about 'tiles' in p5play
    * 5 parameters
      1. A string/array which represent a single row
      2. x-coordinate of the first tile
      3. y-coordinate of the first tile
      4. horizontal spacing between tiles
      5. vertical spacing between tiles
* I plan on watching more videos and trying to make a bigger project  
   
### 12/16/24
* I tried to make a border/field [here](https://jsbin.com/yeducegohe/edit?js) but decided to change to just a "floor"/lines in a new project

### 12/31/24
* Worked on my project which is possibly an [MVP](https://jsbin.com/kigahihipu/edit?js,output)
  * Added the 'field'
  * Two players which are the balls on the ends of the field
    * "player1" moves with "WASD"
    * "player2" moves with "Arrowkeys"
  * The circle in the middle is the "ball"
    * bounces off the walls when it collides
  * I plan on making this project more better
    * add time with a limit
    * add scoreboard with a limit
    * make it so when " " is pressed and a player collides with the ball, the ball will moves away
    * when the ball crosses the "net" it will give the player a goal 

### 1/12/25
* Continued to add to my previous project [here](https://jsbin.com/pobipetuya/edit?js,output)
  * I added a score for player1(score1) and player2(score2)
  * increases when the ball's position is inside the "field" lines at the opposite vertical "border" ends.
  * I plan on added a limit and making it appear on the screen rather than the console
* Also tried to add a timer [here](https://jsbin.com/ridesodayu/edit?js,output)
  * I need to change it so it counts up
  * I also need to get a better understanding of how it works

<!--
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->
