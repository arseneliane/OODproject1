SurveyApp
# Survey Application

## Overview

This Java-based Survey Application was created for educational purposes. It allows users to create, take, and analyze surveys. The application supports three types of users:

1. **SurveyMaker** - Creates surveys by adding questions.
2. **SurveyTaker** - Takes the available surveys and submits responses.
3. **DataAnalyst** - Generates a report based on collected responses.

The application ensures multiple users can participate in the survey-taking process.

## Features

- **Survey Creation:**

  - A SurveyMaker can create surveys with multiple questions.
  - Supports Multiple Choice Questions (MCQ) and True/False questions.

- **Survey Taking:**

  - A SurveyTaker can answer available surveys.
  - Responses are stored in a structured format.

- **Survey Analysis:**

  - A DataAnalyst can generate a report showing the percentage of users selecting each answer.

## How It Works

1. The user is prompted to select a role:

   - "SurveyMaker" to create a survey.
   - "SurveyTaker" to take an existing survey.
   - "DataAnalyst" to generate and view reports.

2. **SurveyMaker Flow:**

   - Enters survey details (name, ID, theme).
   - Adds multiple-choice or true/false questions.
   - Specifies the number of survey takers.

3. **SurveyTaker Flow:**

   - Selects a survey and provides responses.
   - Answers are stored in a 2D array.

4. **DataAnalyst Flow:**

   - Processes survey responses.
   - Displays statistics (e.g., percentage of responses per answer choice).

## Technologies Used

- Java 
- Eclipse (recommended for development)
- Object-Oriented Programming (OOP) concepts

## Classes and Their Relationships

- **SurveyMaker (inherits User)** → Creates surveys.
- **SurveyTaker (inherits User)** → Takes surveys and stores responses.
- **DataAnalyst (inherits User)** → Analyzes and reports survey results.
- **Survey** → Represents a survey, contains questions.
- **Question (abstract class)** → Base class for different question types.
  - **MCQ (inherits Question)** → Multiple-choice question.
  - **TrueFalse (inherits Question)** → True/False question.
- **Response** → Represents survey answers.

## How to Run the Project

1. Open the project in Eclipse or any Java IDE.
2. Compile and run the `Main.java` file.
3. Follow the on-screen prompts to create, take, and analyze surveys.

## Example Output

```
Are you a SurveyMaker or SurveyTaker? (Enter 'SurveyMaker' or 'SurveyTaker')
> SurveyMaker
Enter Survey Name: Favorite Pets
Enter Survey ID: 101
Enter Survey Theme: Animals
Add a Question (MCQ/TrueFalse)? Enter 'exit' to stop:
> MCQ
Enter Question ID: 1
Enter Question Text: What is your favorite pet?
Enter Number of Choices: 3
Enter Choice 1: Dog
Enter Choice 2: Cat
Enter Choice 3: Bird
How many people will take the survey?
> 2

Survey Taker 1:
Enter your username: John
Answer Question 1: Dog

Survey Taker 2:
Enter your username: Jane
Answer Question 1: Cat

Generating Report...
Survey: Favorite Pets
Question 1: What is your favorite pet?
Dog: 50% answered
Cat: 50% answered
Bird: 0% answered
```

## Future Enhancements

- Add user authentication.
- Store survey results in a file or database.
- Implement a graphical user interface using javafx and JDK.

## Authors

Lea Saleh

Arsen Eliane

Johnny Geagea

