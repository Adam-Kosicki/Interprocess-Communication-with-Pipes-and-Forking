# Interprocess-Communication-with-Pipes-and-Forking

TThis project involves creating a communication-based number-guessing game between a user and a computer simulation using C programming. The project is divided into two main components: the communication setup and the number-guessing game itself.

Communication Setup:
The first program sets up a communication mechanism between two processes, namely the user process and the computer simulation process. It uses pipes to establish this communication. The program creates two sets of pipes, one for communication from the user to the computer and another for communication from the computer to the user. A fork is used to create the two processes, with one becoming the parent process responsible for the user interaction and the other becoming the child process responsible for the computer simulation.

Number-Guessing Game:
The second program is a simple number-guessing game implemented within the computer simulation process. The computer selects a target number between a specified range (e.g., 1 to 100). It then interacts with the user process through the pipes, displaying midpoints of the range and receiving input from the user about whether the guessed number is lower, equal to, or higher than the target number. The game continues until the user provides the correct answer, upon which a "Great game!" message is displayed, or until the user enters an invalid response, prompting an error message.

By combining the two programs, the project creates an interactive environment where the user and the computer engage in a number-guessing game. The communication setup using pipes enables data exchange between the two processes, allowing the computer to present guesses and receive feedback from the user. This project provides a hands-on exploration of process communication and interactive program design using C programming concepts.
