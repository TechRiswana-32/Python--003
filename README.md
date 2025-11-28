# Python--003
### 🎮 Python Interactive Program – Guessing Game, Multiplication Table & BMI Calculator

This project combines three interactive Python applications in one file:

✔ Number Guessing Game
✔ Multiplication Table Generator
✔ BMI (Body Mass Index) Calculator

Each section demonstrates Python fundamentals including input handling, loops, conditionals, functions, and error checking.

🔢 Part 1: Number Guessing Game

The program generates a random number from 1 to 10.
The user has 4 attempts to guess the number.

secret_number = random.randint(1, 10)
attempts = 4

while attempts > 0:
    try:
        guess = int(input("Guess the number (between 1 and 10): "))
    except ValueError:
        print("Please enter a valid number.")
        continue


🔸 If the guess is correct → 🎉 success
🔸 If wrong → user gets hints (“Too high” / “Too low”)
🔸 If out of attempts → game ends with failure message

✖️ Part 2: Multiplication Table Generator

User inputs a number.
Program prints multiplication table from 1 to 10.

number = int(input("Enter the number for which you want the multiplication table: "))

print(f"\nMultiplication Table for {number}:")
for i in range(1, 11):
    print(f"{number} x {i} = {number * i}")


Example output:

5 x 1 = 5
5 x 2 = 10
...
5 x 10 = 50

🧍 Part 3: BMI Calculator

User inputs:

weight in kg

height in cm

BMI formula:

𝐵
𝑀
𝐼
=
𝑤
𝑒
𝑖
𝑔
ℎ
𝑡
ℎ
𝑒
𝑖
𝑔
ℎ
𝑡
(
𝑚
)
2
BMI=
height(m)
2
weight
	​

def calculate_bmi(weight, height_cm):
    height_m = height_cm / 100
    bmi = weight / (height_m ** 2)
    return bmi


BMI is then classified:

BMI Range	Category
< 18.5	Underweight
18.5–24.9	Normal
25–29.9	Overweight
30–34.9	Obesity Class I
35–39.9	Obesity Class II
40+	Obesity Class III
✔️ Concepts Practiced in This Program
Concept	Usage
Loops	while, for
User input	input(), numeric conversion
Error handling	try / except
Random number generation	random.randint()
Functions	BMI calculation & classification
Conditional logic	if-elif-else
Data validation	checking numeric input & range
▶️ How to Run

Install Python 3

Save the script as:

app.py


Run:

python app.py


If you want, I can also:
✔ clean + refactor your code
✔ add comments for beginners
✔ convert to GUI (Tkinter)
✔ build a web version (Flask/HTML)
✔ format outputs with colors

Just tell me what you want next.

c

ChatGPT can make mistakes. Check important info. See Cookie Prefe
