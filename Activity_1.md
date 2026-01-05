# ACTIVITY 1: 🧙‍♂️ Build an RPG Character

In this lab, you will practice the basics of **Python 🐍** by building a small app that creates a character for an RPG adventure ⚔️🎲.

---

## 🎯 Objective

Fulfill the user stories below and get all the tests to pass to complete the lab ✅.

---

## 📘 User Stories

- You should have a function named **create_character**.
- The function should accept, in order:
  - a **character name**
  - three stats:
    - **strength**
    - **intelligence**
    - **charisma**

---

## 🏷️ Character Name Validation

The character name must follow these rules:

- If the character name is **not a string**, the function should return:  
  **The character name should be a string.**

- If the character name is an **empty string**, the function should return:  
  **The character should have a name.**

- If the character name is **longer than 10 characters**, the function should return:  
  **The character name is too long.**

- If the character name **contains spaces**, the function should return:  
  **The character name should not contain spaces.**

---

## 📊 Stats Validation

The stats (**strength**, **intelligence**, and **charisma**) must follow these rules:

- If **one or more stats are not integers**, the function should return:  
  **All stats should be integers.**

- If **one or more stats are less than 1**, the function should return:  
  **All stats should be no less than 1.**

- If **one or more stats are more than 4**, the function should return:  
  **All stats should be no more than 4.**

- If the **sum of all stats is different from 7**, the function should return:  
  **The character should start with 7 points.**

---

## 🧾 Successful Character Output

If all values pass validation, the function should return a **string with four lines**:

1. The **first line** contains the character name
2. Lines **2–4** represent the stats in this order:
   - **STR**
   - **INT**
   - **CHA**

Each stat line must:
- Start with the stat abbreviation
- Be followed by a space
- Show a number of **full dots (●)** equal to the stat value
- Show **empty dots (○)** to reach a total of **10 dots**

📌 Example:  
If a stat value is **3**, it should display **3 full dots** followed by **7 empty dots**.

---

## 🧪 Example Output

For the following input:

- Name: `ren`
- Strength: `4`
- Intelligence: `2`
- Charisma: `1`

The function should return:
```text
ren
STR ●●●●○○○○○○
INT ●●○○○○○○○○
CHA ●○○○○○○○○○
```


---

## ⚠️ Important Note

While **str** and **int** are common abbreviations for stats, they are **reserved keywords in Python** and **must not be used as variable names** ❌.

---


CODE:

```python

