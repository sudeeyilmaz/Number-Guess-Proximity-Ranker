# 🎯 Number Guess Proximity Ranker

A Java-based command-line tool that turns a standard number guessing game into a **proximity analysis tool**. Instead of just checking for the correct answer, this program evaluates 5 distinct user guesses and ranks them from "closest" to "furthest" relative to a randomly generated target number.

## 🚀 Features

* **Random Generation:** Generates a random integer between **1 and 100**.
* **Batch Input:** Accepts 5 sequential guesses from the user.
* **Proximity Calculation:** Uses `Math.abs()` to calculate the absolute distance (difference) between each guess and the target number.
* **Custom Sorting Logic:** Implements a manual insertion-style sorting algorithm to rank the guesses based on their proximity deviations.
* **Detailed Reporting:** Outputs the target number and lists all guesses sorted by accuracy.

## 🛠️ How It Works

1.  The system picks a secret number (e.g., `42`).
2.  The user inputs 5 different numbers (e.g., `40`, `90`, `10`, `43`, `50`).
3.  The program calculates the deviation for each:
    * `40` -> diff: 2
    * `90` -> diff: 48
    * `10` -> diff: 32
    * `43` -> diff: 1
    * `50` -> diff: 8
4.  It sorts these values and prints the results starting with the closest guess (in this case, `43`).

## 💻 Usage

To run this project, ensure you have the Java Development Kit (JDK) installed.

```bash
# Compile the program
javac tahmin_oyunu.java

# Run the application
java tahmin_oyunu
