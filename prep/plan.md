# Plan

## Tool: p5play
## Product: Soccer game

---

## Timeline

#### MVP

- [ ] Make a fixed soccer field/boundaries the ball and the players can't go through --> static collider (deadline: 2/20)
- [ ] Create a scoreboard with a timer next to it (deadline: 2/24)
  - [ ] make the score appear on the game and only increase when there is a "goal" (the ball goes into the net)
- [ ] Everytime there is a goal, reset the game to the starting setup (ball in the middle, players on opposite ends) (deadline: 3/17)
- [ ] Add a limit to the timer and scores (deadline: 3/5)
  - [ ] if the goals limit is reached by either player before the time ends, the game ends and resets
  - [ ] if the time runs out and the game is not tied but the score limit has not been reached, the game ends
  - [ ] if the the game is tied and the time runs out, the game goes into extratime until someone scores 
- [ ] Make is so when the ball and player collide and the player presses "space" there is a force on the ball (deadline: 3/10)
  - [ ] The ball goes in the direction of the force
- [ ] Set a fixed velocity for both players that is equal (deadline: 2/21)
  - [ ] The keypressed determines the direction of the velocity

#### Beyond MVP

- [ ] Task
  - [ ] Subtask


<!-- EXAMPLE

## Tool: APIs
## Product: Green Glass Door riddle app

## Timeline

### MVP

- [ ] Front-end
  - [x] Webpage to collect input from user (deadline: 4/15)
  - [ ] Webpage to display "yes, but a ___ can't" or "no, but a ___ can" (deadline: 5/1)
- [x] Back-end
  - [x] Use regex to test whether or not the word can go through the GGD (deadline: 3/1)
  - [x] Use the Twinword API to find related words (deadline: 3/15)
    - [ ] Iterate through the words until an opposite example can be found (deadline: 4/1)

#### Beyond MVP

- [ ] Use another API to make sure the opposite example is a noun
- [ ] Automate notification of API limit to make sure I don’t exceed free quota
- [ ] A multiple choice quizzer that will test the user’s knowledge of the solution

-->





<!-- DO NOT USE THIS YET

| Name | Glows | Grows |
| -------- | ------- | ------- |
|   |   |
|   |   |
|   |   |
|   |   |
|   |   |
|   |   |

-->
