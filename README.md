# Nim Project

## Problem Statement

In the game of nim two players compete to be the last one to grab all remaining matches from a set of piles.

To start the game, three heaps of matches are made:

- Heap A: 3 matches
- Heap B: 4 matches
- Heap C: 5 matches

Each player alternates turns grabbing any amount of matches from 1 heap. They may not mix and match matches from different heaps.

The game ends when a player successfully takes the last match, and leaves the opponent unable to take a match.

Another version of the game exists where the last player to take a match loses as well. Either version of the game is a valid submission for this project.

### An example game

| Heap A | Heap B | Heap C | Move |
| - | - | - | - |
| 3 | 4 | 5 | Game begins |
| 1 | 4 | 5 | Bob takes 2 from A |
| 1 | 4 | 2 | Alice takes 3 from C |
| 1 | 3 | 2 | Bob takes 1 from B |
| 1 | 2 | 2 | Alice takes 1 from B |
| 0 | 2 | 2 | Bob takes entire A heap, leaving two 2s |
| 0 | 1 | 2 | Alice takes 1 from B |
| 0 | 1 | 1 | Bob takes 1 from C leaving two 1s. (In misère play he would take 2 from C leaving (0, 1, 0).) |
| 0 | 0 | 1 | Alice takes 1 from B |
| 0 | 0 | 0 | Bob takes entire C heap and wins |

### Requirements

- Your game must be a proper implementation of the game of nim.
- You must user proof any player input. 
    - if the user enters something invalid, tell them it was not valid and prompt them again.
- You must display the current state of the game before any player takes a turn.

You may add the additional features as bonus:

- Allow the user to play again without re running the program. (to earn this point, you must ask the player if they want to play again, not just loop forever)
- Allow the user(s) to select custom values for each of the heaps before playing.
- Allow the user(s) to select a game mode (normal or misere play)

## Input Description

You are defining the input and output yourself. Please include a description of your controls.

## Sample Input/Output

You are defining the input and output of the game. There is no defined input and output, however, the following is just ***one example*** of a working game.

```
Welcome to the game of Nim!

Currently the heaps are as follows:

   Heap A: | | |
   Heap B: | | | |
   Heap C: | | | | |
   
Player 1, which heap would you like to take from? A
How much? 2

Currently the heaps are as follows:

   Heap A: |
   Heap B: | | | |
   Heap C: | | | | |
   
Player 2, which heap would you like to take from? C
How much? 6

That is not a valid move!

Player 2, which heap would you like to take from? C
How much? 5

Currently the heaps are as follows:

   Heap A: |
   Heap B: | | | |
   Heap C:
   
Player 1, which heap would you like to take from? D

That is not a valid move!

Player 1, which heap would you like to take from? B
How much? 3

Currently the heaps are as follows:

   Heap A: |
   Heap B: |
   Heap C:
   
Player 2, which heap would you like to take from? A
How much? 0

That is not a valid move!

Player 2, which heap would you like to take from? A
How much? 1

Currently the heaps are as follows:

   Heap A:
   Heap B: |
   Heap C:

Player 1, which heap would you like to take from? B
How much? 1

Currently the heaps are as follows:

   Heap A:
   Heap B: |
   Heap C:

Congrats Player 1! You won!

```

## Submission

Please submit the following to google classroom:

1. `Main.java`
    * Hover over `Main.java`.
    * Click the three dots to the right of the file name.
    * Click `Download`.
    * Upload the downloaded file to google classroom.
2. A link to your replit project

## Rubric

<table>
<tbody>
  <tr>
    <td valign="top"><b>Coded Solution</b><br><br>The coded solutions works correctly with no syntax, logic, or run-time errors.</td>
    <td valign="top"><b>8pts</b><br><br>* The submitted code compiles successfully. <br><br>* The submitted program is free of run-time and logic errors. <br><br>* The submitted program returns the anticipated output for all input tested.
</td>
    <td valign="top"><b>4pts</b><br><br>* The submitted program compiles successfully. <br><br>* The submitted program includes run-time and/or logic errors that result in correct output. <br><br>* The submitted program returns the anticipated output for most (but not all) input tested.
</td>
    <td valign="top"><b>2pts</b><br><br>* A program is submitted but it fails to compile. <br><br><b><em>or</em></b> <br><br>* The submitted program compiles correctly. <br><br>* The submitted program includes run-time and/or logic errors that result in incorrect output. <br><br>* The submitted program returns the anticipated output for less than half of the input tested.
</td>
    <td valign="top"><b>0pts</b><br><br>* A program solution is not submitted.
</td>
  </tr>
  <tr>
    <td valign="top"><b>Target Concepts</b><br><br>The program effectively uses the intended target concepts.</td>
    <td valign="top"><b>8pts</b><br><br>* The program effectively uses the target concepts being discussed in class or outlined within the project specifications for the given problem situation.
</td>
    <td valign="top"><b>4pts</b><br><br>* The program incorrectly uses the target concepts being discussed in class or outlined within the project specifications for the given problem situation. <br><br>* Moderate effort to use the target concepts is evident.
</td>
    <td valign="top"><b>2pts</b><br><br>* The program incorrectly uses the target concepts being discussed in class or outlined within the project specifications for the given problem situation. <br><br>* Minimal effort to use the target concepts is evident.
</td>
    <td valign="top"><b>0pts</b><br><br>* A program solution is not submitted. <br><br><b><em>or</em></b><br><br> * No attempt was made to use the target concepts being discussed in class or outlined within the project specifications for the given problem situation.
</td>
  </tr>
  <tr>
    <td valign="top"><b>User Interface</b><br><br>The program produces output that is easy for the user to read.</td>
    <td valign="top"><b>2pts</b><br><br>* Output demonstrates appropriate spacing for best user readability. <br><br>* Output contains no spelling or grammatical errors.
</td>
    <td valign="top"><b>1pts</b><br><br>* Output includes minor spacing problems which results in information which is inconsistent or confusing. <br><br>* Output contains minor spelling or grammatical errors.
</td>
    <td valign="top"><b>0pts</b><br><br>* A program solution is not submitted. <br><br><b><em>or</em></b> <br><br>* Output includes major spacing problems which is severely inconsistent or confusing. <br><br>* Output contains major spelling or grammatical errors.
</td>
  </tr>
  <tr>
    <td valign="top"><b>Readability of Code</b><br><br>The program code is documented and formatted for human readability.</td>
    <td valign="top"><b>2pts</b><br><br>* The submitted solution includes the required header documentation (name, date, purpose). <br><br>* Header documentation includes appropriate modification comments if the submitted solution is a modification to a previously submitted program. <br><br>* Code is properly formatted. Open and close brackets are properly aligned and code within the brackets is appropriately indented. <br><br>* All variables are self-documented (i.e. named in such a way that the name indicates the purpose of the variable).
</td>
    <td valign="top"><b>1pts</b><br><br>* The submitted solution includes the some, but not ALL, of the required header documentation (name, date, purpose). <br><br>* In the case of modifications to a previously submitted program, modification comments are missing or incomplete. <br><br>* Code is unformatted and difficult to follow. Brackets aren't aligned and/or code within brackets is not indented. <br><br>* Numerous variable names are ambiguous (i.e. x) and do not indicate the purpose of the variable.
</td>
    <td valign="top"><b>0pts</b><br><br>* A program solution is not submitted. <br><br><b><em>or</em></b> <br><br>* The submitted solution includes no documentation of any kind.</td>
  </tr>
</tbody>
</table>
