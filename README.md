# Math-app
import random

def multiplication_exercise():
    score = 0
    num_questions = 5

    print("🧠 Welcome to the Multiplication Practice!")
    print("You will be asked", num_questions, "questions.\n")

    for i in range(num_questions):
        a = random.randint(1, 12)
        b = random.randint(1, 12)
        correct_answer = a * b

        try:
            user_answer = int(input(f"Question {i + 1}: What is {a} x {b}? "))
        except ValueError:
            print("❌ Invalid input. Please enter a number.")
            continue

        if user_answer == correct_answer:
            print("✅ Correct!\n")
            score += 1
        else:
            print(f"❌ Wrong! The correct answer is {correct_answer}\n")

    print(f"🎉 You got {score} out of {num_questions} correct!")
    from zipfile import ZipFile

# File contents
main_py = """import random

def multiplication_exercise():
    score = 0
    num_questions = 5

    print("🧠 Welcome to the Multiplication Practice!")
    print("You will be asked", num_questions, "questions.\\n")

    for i in range(num_questions):
        a = random.randint(1, 12)
        b = random.randint(1, 12)
        correct_answer = a * b

        try:
            user_answer = int(input(f"Question {i + 1}: What is {a} x {b}? "))
        except ValueError:
            print("❌ Invalid input. Please enter a number.")
            continue

        if user_answer == correct_answer:
            print("✅ Correct!\\n")
            score += 1
        else:
            print(f"❌ Wrong! The correct answer is {correct_answer}\\n")

    print(f"🎉 You got {score} out of {num_questions} correct!")

# Run the exercise
multiplication_exercise()
"""

readme_md = """# 🧮 Math Practice App

A simple Python-based terminal quiz to practice multiplication skills.

## 💻 How to Run

1. Download or clone this repo.
2. Make sure you have Python installed.
3. Open a terminal and run:

```bash
python main.py

# Run the exercise
multiplication_exercise()
