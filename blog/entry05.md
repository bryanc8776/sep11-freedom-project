# Entry 5: MVP
##### 4/27/25

### Content
Since my last entry, I have continued to make progress and learn my tool, [p5play](https://p5play.org/learn/). The main thing I got from p5play was the `applyForce()` concept which I used to apply a force to the ball when a player collides with it and presses their respective key.
``` JS
if(player1.colliding(ball) && kb.presses("x")){
    if(kb.pressing('d')){
        ball.applyForce(200)
    } else if(kb.pressing('a')){
        ball.applyForce(-200)
    }
}
if(player2.colliding(ball) && kb.presses("l")){
    if(kb.pressing('arrowRight')){
        ball.applyForce(200)
    } else if(kb.pressing('arrowLeft')){
        ball.applyForce(-200)
    }
}
```
This mainly works to make the ball be kicked in the left or right direction.


I mainly had to figure out how to update the score of the player that made a goal and make the timer increase to 5 minutes. After a little struggle, I used conditionals to check when the ball passes the nets and to determine the value of the timer.
``` JS
if(ball.x < 250 && ball.x > 200 && ball.y > 300 && ball.y < 500) {
    score2++;
    reset();
} else if(ball.x > 1550 && ball.x < 1600 && ball.y > 300 && ball.y < 500) {
    score1++;
    reset();
}
text(score1 + ":" + score2, width/2 + 100, height/10)

if (timerValue < 10) {
    text("0:0" + timerValue, width / 2 -100, height / 10);
}
if (timerValue >= 10 && timerValue <60) {
    text('0:' + timerValue, width / 2 -100, height / 10);
}
if(timerValue >=60 && timerValue < 70){
    text('1:0' + timerValue % 60, width / 2 -100, height / 10);
}

```
The code `text('text to show', x, y)` makes the timer and score be displayed in my game. In the end, I feel like I made a good MVP, but I still need to make some improvements. [Here](https://bryanc8776.github.io/sep11-freedom-project/) is the link to my game.

### Engineering Design Process
I completed my MVP and tested it to make sure it works relatively well. I am now in step 7 of the EDP which is to improve my project as needed. I plan to add a little more to it and make changes to make sure it runs better.

### Skills
I have improved on **Time management** and **Problem decomposition**. Over Spring Break, I had a couple of assignments from other classes along with the MVP. I decided to do the other assignments first in the first couple of days since they took less time and then I could focus on finishing my MVP. In order to complete my MVP, I also needed to do many things so I decided to separate them into different tasks. First I focused on getting the timer to work and run properly until 5 minutes and making the score increase. Then I focused on making ball and player positions reset when there is a goal and if there were 3 goals or the timer ends the whole game(timer, score, and positions) would reset.

[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)
