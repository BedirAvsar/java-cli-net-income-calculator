# Java CLI Net Income Calculator

A simple command-line Java application that calculates monthly net income for a small shop.  
The program takes item revenues, staff expenses, and other costs as input and outputs the final net profit for the month.

---

## 🚀 Features

- Read revenues of multiple items
- Read staff salary expenses
- Read operational expenses
- Calculate total income
- Calculate total expenses
- Compute final net income
- Display formatted output in the console

---

## 📦 Project Structure

```
My First Project with Java/
└── task/
    └── src/
        └── calculator/
            ├── Main.java
            └── IncomeCalculator.java
```

---

## 📌 How It Works

### 1️⃣ User inputs:
- Product revenues
- Staff salaries
- Other expenses

### 2️⃣ Program processes values:
```java
int netIncome = totalRevenue - (staffExpenses + otherExpenses);
```

### 3️⃣ Final result is printed:
```
Net Income for this month: $X
```

---

## 🧠 Example Code (Main.java)

```java
public class Main {
    public static void main(String[] args) {

        IncomeCalculator calc = new IncomeCalculator();

        calc.readRevenues();
        calc.readStaffExpenses();
        calc.readOtherExpenses();

        int net = calc.calculateNetIncome();

        System.out.println("Net Income for this month: " + net);
    }
}
```

---

## 🧩 What I Learned

- Basic Java syntax
- Console input (Scanner)
- Arithmetic operations
- Organizing code into multiple classes
- Using methods to separate logic
- Printing formatted output
- Running Java apps with Gradle

---

## ▶️ Run Instructions

**Build:**
```
./gradlew build
```

**Run:**
```
./gradlew run
```

If running manually:

```
javac Main.java
java Main
```

---

## 📄 Notes

This project was originally created as part of Hyperskill’s beginner Java track and then structured more cleanly for GitHub.
