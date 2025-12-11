Logic point A: health

| Boundary input | Why it’s a boundary | Test data example | Expected outcome |
| :---- | :---- | :---- | :---- |
| Health \= 0 | To see if the player dies at 0 hp | Player still alive at 0 hp when should be dead | Player dies at 0 hp |
| Health below 0 | To see if negative hp is even possible | Player at \-5 hp and still alive \- shouldn't be possible | Player can’t go below 0 hp |
| Health above 100 | To make sure there is a maximum health | Player has 120 hp but shouldn’t go over 100 | Player can only have 100 hp at most |

Logic point B: timer

| Boundary input | Why it’s a boundary | Test data example | Expected outcome |
| :---- | :---- | :---- | :---- |
| Timer \= 0 | To see if a game level ends when the timer reaches 0 | Player still in-play even when timer hit 0 | Game level ends |
| Timer below 0 | To see if a recorded negative time is even possible | Timer is at \-15 when level should be over at 0 | Game over when timer reaches 0 |

Logic point C: inventory

| Boundary input | Why it’s a boundary | Test data example | Expected outcome |
| :---- | :---- | :---- | :---- |
| Inventory spaces left \= 0 | To see if items can be picked up when 0 spaces are left | Player picks up a fifth item when there are only 4 spaces | Player can’t pick up fifth item |
| Inventory spaces \= 4 | To make sure player can have at least 4 items in inventory | Player can’t pick up more than 2 | Player should be able to pick up 2 more items |
