Overview:
The AlgoCoins class simulates a coin reward system designed for an educational platform. It helps manage coin allocations based on users' activities such as completing questions, assignments, and participating in contests. The class offers a streamlined way to track progress and reward users for achievements and efficient performance.

Key Features
1. Question Completion Rewards: Earn coins by completing individual questions.
2. Assignment Completion Bonus: Earn a bonus for finishing all questions in an assignment.
3. Monthly Completion Bonus: Get additional coins for completing all assignments within a month.
4. Contest Rewards: Earn coins for attempting questions in contests, with bonuses for correct answers and faster completion.

Class and Method Descriptions
Class: AlgoCoins

Attributes
coins: Tracks the total number of coins earned by the user (initialized to 0).

Methods
1. complete_question_assignment: Adds 20 coins for each question completed in an assignment.
2. complete_assignment: Adds a 50-coin bonus for completing all questions in a single assignment.
3. complete_all_assignments: Adds a 150-coin bonus for completing all assignments within a specified period (e.g., a month).
4. attempt_question_contest(correct=False, submission_attempts=0): Manages coin rewards for contest question attempts:
  If answered correctly, a base 30-coin bonus is added.
  Additional bonuses are awarded based on submission attempts:
  0 attempts: +30 coins
  1 attempt: +20 coins
  2 attempts: +10 coins
5. complete_contest: Adds a 100-coin bonus for answering all contest questions correctly.
6. complete_almost_all_contest(wrong_questions=1): Awards coins for near-perfect performance in a contest:
   1 wrong question: +80 coins
   2 wrong questions: +60 coins
   More than 2 wrong questions: No bonus
7. total_coins: Returns the total coins collected.
