# C++ Math Quiz Game

This is a console-based *Math Quiz Game* written in C++. The game generates arithmetic questions of varying difficulty and tests the user's math skills.

## Features

- Multiple difficulty levels:
  - Easy
  - Medium
  - Hard
  - Mixed (random difficulty)
- Arithmetic operations:
  - Addition (+)
  - Subtraction (-)
  - Multiplication (Ã—)
  - Division (/)
  - Mixed (random operation)
- Feedback for correct and incorrect answers
- Colored screen feedback:
  - Green background for correct answers
  - Red background and alert sound for wrong answers
- Score tracking (right and wrong answers)
- Pass/fail result at the end

## How It Works

1. The program initializes a set number of math questions.
2. For each question, the user is prompted to input an answer.
3. The program checks the answer and gives immediate feedback.
4. At the end, it displays the total score and whether the user passed.

## Code Overview

- **enum enQuestionsLevel**: Defines difficulty levels.
- **enum enOperationType**: Defines operation types.
- **struct stQuestion**: Represents a single quiz question.
- **struct stQuizz**: Represents the entire quiz session.
- *Key functions*:
  - GenerateQuestion() â€” Creates a question based on selected difficulty and operation.
  - AskAndCorrectQuestionListAnswers() â€” Asks questions and evaluates answers.
  - PlayMathGame() â€” Main quiz logic controller.

## Build & Run

### Requirements:
- C++ compiler (like g++)
- Compatible with Windows (uses system("color") for screen feedback)

### Compile:
bash
g++ -o MathQuiz MathQuiz.cpp


### Run:
bash
./MathQuiz


## Sample Output


Question [1/5]
7 + 3 = 10
Correct!

...

Quiz Completed! Right Answers: 4, Wrong Answers: 1
You Passed the Quiz!


## Notes

- The game uses srand(time(NULL)) to ensure randomization.
- Division by zero is safely handled by returning 0.
- You can change the number of questions or difficulty level by editing PlayMathGame().

## License

This project is open-source and available for learning and personal use.
