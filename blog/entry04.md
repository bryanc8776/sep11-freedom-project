# Entry 4: Learning Continued
##### 3/10/25

### Content
Over the past weeks, I have been trying to work on my MVP for my game, which is the minimum I need to make it work. To understand how much I need to make a functional soccer game and keep track of my progress, I made a [plan](../prep/plan.md). I have made some progress towards my MVP, but still need to learn and make a lot.

![Screenshot 2025-03-16 154027](https://github.com/user-attachments/assets/f19a88f5-a5a7-42e3-94ae-8f7f4f4c8084)
![Screenshot 2025-03-16 154756](https://github.com/user-attachments/assets/134a0e80-b539-4ab9-8ca6-3f4b12cf4d1c)

This is what I have done so far. I set the borders and the field lines to 'white' with `field.color` and `border.color`, added goals/nets for each player, and added a scoreboard which tells the time and score. I also made the time increase with this code:

```JS
function timeIt() {
  if (timerValue > 0) {
    timerValue++;
  }
}
```
It makes the `timerValue` increase by 1 second every second. I still need to make a timer that fits my game.

#### Next Steps
I haven't made the progress I wish I had, so I really need to focus on reviewing the [p5play](https://p5play.org/learn/) concepts and try to catch up with my plan or make some changes and make sure I meet those deadlines. I have to make the time appear correctly and make it show on the scoreboard as well as the score which should only increase when the ball goes through the net.

### Engineering Design Process
I am currently on steps 2 and 3 of the EDP. I am working on my MVP, but still need to learn more about the code of p5play to make my game work and be more interactive/advanced. I also need to continue following my plan and make some changes so I can make sure I finish my MVP.

### Skills
The skills I have improved on are **Communication** and **Collaboration**. In the past week, I had to do a project in APUSH with a group and the DOM Challenge in SEP with my partner. In APUSH, I had to talk with my partners, making sure we all knew what we were doing and preparing to present to our classmates. In my presentation, I felt that I did a good job, trying to give as much details as I could remember. In SEP, I had to make sure my partner and I were communicating through Slack and in class to prevent merge conflicts.


[Previous](entry03.md) | [Next](entry05.md)

[Home](../README.md)
