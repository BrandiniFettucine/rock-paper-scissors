# rock-paper-scissors
This is a small project started with the guidance of The Odin Project.

In this project, I was tasked with creating a program to play rock paper scissors using javascript in an html document. Below, I will walk through the exact order I progressed through the task.

I started off by creating the computerPlay() function which is what is used to generate the computer's choice of rock, paper, or scissors. To begin, the function generates a random number from 0 to 2, and assigns that value to an arbitrary variable, in this case, x is used. I then used a  switch statement to return strings "rock", "paper", or "scissors", depending on the random number generated.

To get the user's response, I created the variable userInput which stores the value from a prompt. I also added a .toLowerCase() function to the end of this prompt, so that the user input would be case insensitive.

After this, I created the playRound() function which takes parameters userInput and computerSelection. This function's purpose is to return a win, lose, or draw string based on the user's input (userInput) and the computer's decision (computerSelection). This was done combining if/else statements with switch statements.

Finally, I created the game() function which takes the user's input and compares it to 5 computer generated responses. This was done using a for loop to repeat the playRound function 5 times. Also for each loop, the computerPlay() function was run and it's value was stored in the computerSelection variable, which allowed for a random result 5 times.

I also realized that I needed to adjust the playRound() function to keep track of wins and losses, so I added a winCounter variable set to 0 to the beginning of the code, and used the ++ syntax to increase the winCounter value by one if the player won, and the -- syntax to decrease the winCounter value by one if the player lost.

Finally, I added an if statement in the game() function which used the || operators. This if statement checks if the user inputted rock, paper, or scissors. If one of those options were not inputted, then instead of playing the rounds 5 times and deciding a winner, it instead returns the string "Please type in rock, paper, or scissors.".-
