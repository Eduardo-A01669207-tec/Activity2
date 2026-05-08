## Original Snake.py

How to run the game: python3 snake.py

## List of changes for this file:

- The food can now move independently one step at a time in a random direction, without leaving the playing area.
- Each time the game runs, the snake and the food have randomly selected different colors from a set of 5 colors (excluding red).

## Change 1

The food movement was changed so that instead of teleporting to a random position, it now moves one step at a time in a random direction (up, down, left, or right). A new function called moveFood() was added. Inside this function, a list of 4 vectors is defined, each representing a possible step direction. Using the choice() function from the random module, one of these directions is randomly selected. A copy of the current food position is made, moved in the selected direction, and if the new position is still inside the window boundaries, the food is moved there. This makes the food move more naturally across the screen. Additionally, the window size was changed from setup(420, 420) to setup(600, 600) and the moveFood() timer was added with a 600ms interval.

**Author:** Alejandro Rodriguez Brito

## Change 2

The snake and the food colors were changed so that each time the game is started, they are independently assigned random colors chosen from 5 possible colors. At the top of the code, a list of 5 colors was defined: blue, green, yellow, pink, and purple. Using the sample() function from the random module, 2 random colors are selected from this list and assigned to the snake_color and food_color variables. The snake body is drawn using snake_color and the food using food_color. This makes the game look different every time it is run.

**Author:** Eduardo Arteaga Camacho
