# Entry 2: Learning p5play
##### 12/9/24

### Tool Learning
For the past weeks, I have been learning more about my tool, ***p5play***. I have made a lot of progress in understanding and trying out different features of ***p5play***. The main way I have been tinkering is through mini-projects, watching videos, and reviewing the documentations.

#### Tinker:
I tried to do some mini-projects with the concepts as I reviewed them so I can get a better understanding of how they work. 
* [Here](https://jsbin.com/genizumemi/edit?js,output) is one of the main projects I worked on which is mainly about *Advanced Movements*. I used the starter code from [here](https://p5play.org/learn/sprite.html?page=10) and later added more things. It included concepts such as `sprites`, which were a "drone" and a "floor", `world.gravity`, `collider`, `velocity`, and `kb.pressing`. 

```JS
function draw() {
  background(16);
  
  if (kb.pressing('space')) {
    drone.bearing = -90;
    drone.applyForce(6);
  }
  if (kb.pressing('arrowLeft')) {
    drone.vel.x = -1.5
  } else if (kb.pressing('arrowRight')) {
    drone.vel.x = 1.5
  }
  
  if (drone.colliding(floor)) {
    drone.vel.x=0
  }
  
  if (drone.y < 300 && drone.y >200 && drone.x >700){
    drone.collider = 's'
  }
  if (kb.pressing('z')){
    drone.collider = 'd'
    drone.vel.y = 2;
  }
}
```
Here is my code that affects the direction of the drone's movement and the type of `colliding` it has when it is in different areas and different keyboard keys are pressed.
![Screenshot 2024-12-15 205415](https://github.com/user-attachments/assets/29bbc714-36c9-40ea-84c4-9337964db4a2)
This is when the drone's x-value is greater than 700 and it's y-value is between 300 and 200. It's `collider` becomes `static` so it can't move unless you press `z` which makes it move down and become free as shown in the image below. 
![Screenshot 2024-12-15 205429](https://github.com/user-attachments/assets/d39ded14-4436-42b6-8de1-8269b3fd58bb)

* I also watched [this](https://jsbin.com/gihekoxiyu/edit?js,output) video which basically went over sprites and the values you can include in it. I learned the following:
  * `Sprite(x, y, width, height or 'shape')` is the setup for a sprite declaration to get shapes but you can also add other concepts, in particular `collision`.
  * If you only define the 'width' you get a circle.
  * If you define both 'width' and 'height' you get a square/rectangle.
  * You can set `Sprite()` equal to a variable with `var_name = Sprite(x, y, width, height or 'shape')` to later add properties like this: `var_name.property = value`.

#### FP Winter Break Goal
My goal for the winter break is to have a good time with my family and get some rest. However, I also aim to continue learning and practicing my tool. I plan on trying to create my own project starting from absolute zero and adding many features to it that could possibly make it something like I want my final game to be like or a little more complex than what I have been doing. I plan on doing this in the first couple of days of the break.

### Engineering Design Process
I am currently on stage 2 of the engineering designing process. I am learning about the different code and concepts in ***p5play*** and documenting what I find. After understanding some of the concepts, I try out different code to make mini-projects and get a better sense of how that concept affects the overall project.

### Skills
The skills I have improved on during this time are **How to Learn** and **How to Read**. Throughout learning my tool, I had to go through the documentations over and over again so I can understand the concepts better. I decided to go through the entire document first, then as I went through it again I just skimmed it and looked for the important sections. At some points I also took notes on the important stuff. Along with this, I had to review many things for other subjects like History and Math so I tried many methods to learn the material like taking notes, quizzing myself, and highlighting the most important areas of the documents.

[Previous](entry01.md) | [Next](entry03.md)

[Home](../README.md)
