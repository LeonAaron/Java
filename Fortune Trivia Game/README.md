# Fortune Trivia Game

## Overview
Fortune Trivia Game is a Java-based word guessing game. It presents the player with a series of questions in various categories such as phrases, movies, animals, countries, and more. The player needs to guess the correct answer based on the hint provided. The game is built using Object-Oriented Programming principles, and it features randomization of categories and questions for an engaging experience.

## Features
- Multiple categories for questions (e.g., "Phrase", "Movie Title", "Animal", "Country", etc.)
- Option for random category selection for each round
- A variety of question types to keep the gameplay interesting
- Scoring based on correct answers

## Requirements
To run this game, you'll need:
- **Java 8 or higher** installed on your machine.
- A suitable IDE like **Eclipse** or **IntelliJ IDEA**

## Installation Instructions

### 1. Clone the repository:

To get started, clone the repository using the following command:

```bash 
    git clone https://github.com/LeonAaron/Portfolio.git
 ```

This will clone the entire Java repository to your local machine.


### 2. Navigate to the project folder:

After cloning the repository, navigate to the Fortune Trivia Game folder:

cd Portfolia/Fortune\ Trivia\ Game/


### 3. Open in your IDE:

You can now open this project in any Java-compatible IDE (such as IntelliJ IDEA or Eclipse) to start working with or running the game.

### How to Run the Program 
Open the project in your IDE.
Locate the **MainFortune.java** file in the src directory.
Run the MainFortune class. This will start the game.
After selecting a random prize for the round, the game will automatically present a hint and ask the player to guess the answer. Based on the answer, you will receive feedback on whether the guess was correct or not.

### Game Settings  
Can be customized in MainFortune.py  

Question Categories: The game can randomly select questions from different categories if **Question.generateRandomCategory()** is input.  
                     Can select specific category by inputing category name (Ex. "Movie Title").
                     May use all categories by omitting input.  
Number of Tries: User can customize number of guesses per word.
Number of Turns: Customize total number of turns in a game.
Starting Net Worth: Modify starting net worth. 

**Example Setup**
FortuneGame game = new FortuneGame(questions, 3, 10, 0, "Phrase");

questions: references static attribute within QuestionFortune class that contains all question objects in array list.
3: Total tries per turn.
10: Total turns per game.
0: Starting net worth.
"Phrase": Specific category selection.


Scoring: Players receive points/prizes for every correctly guessed word.      

### Example Gameplay

Example 1 <br>
Hint: "A common greeting." <br>
Answer: "HAVE A GOOD DAY" <br>
Player's Guess: "HAVE A GOOD DAY" <br>
Result: Correct! The player gets a point. <br>

Example 2
Hint: "A blockbuster movie featuring dinosaurs." <br>
Answer: "JURASSIC PARK" <br>
Player's Guess: "JURASSIC PARK" <br>
Result: Correct! The player gets a point. <br>

Example 3 <br>
Hint: "A domesticated animal often kept as a pet, known for its loyalty."   
Answer: "DOG" <br>
Player's Guess: "DOG" <br>
Result: Correct! The player gets a point.


**The main files in the repository are:**

MainFortune.java: The entry point of the game where the game is initialized and played.  
QuestionFortune.java: Defines the structure for each question, including the hint, answer, and category.  
FortuneGame.java: Handles the game logic, including randomly selecting questions and managing the player's score.  


**How the Game Works**

Game Setup: The game initializes a list of QuestionFortune objects, each containing a hint, answer, and category.  
Randomization: At the start of each round, the game randomly selects a category and presents a question from that category.  
Player Interaction: The player is prompted to guess the answer to the question.  
Feedback: The game provides feedback, such as whether the guess was correct or not, and continues until all rounds are completed.  

**If you'd like to customize the game, you can:**

Add more categories: You can add new question categories to the game by adding new QuestionFortune objects with different hints and answers.  
Adjust game settings: Modify the game logic in the FortuneGame class to change the number of rounds, question types, or difficulty.  
Adding New Categories:  
To add a new category, simply create a new QuestionFortune object with the following format:  

new QuestionFortune("Your hint", "Your answer", "Your category");  

For example:  
new QuestionFortune("A country known for its pyramids and ancient civilization.", "EGYPT", "Country");  

**To change the number of rounds or difficulty, modify the FortuneGame class:**  


The first number 3 represents the number of rounds.  
The second number 10 represents the time limit (you can modify this as needed).  
"Phrase" is the default category, which can be adjusted.  
