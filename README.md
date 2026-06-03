# 🚀 C# Exercise Collection (C-codes)

This repository contains a collection of console applications developed in **C# (.NET)**. The projects cover everything from basic programming logic, validations, and list manipulation with LINQ to manual implementations of classic data structures such as Dynamic Stacks.

## 📁 Repository Structure

The repository is composed of the following programs:

* **`MediaSalarial.cs`**: Manager that receives employee data, validates minimum salary limits, and calculates salary statistics.
* **`PilhaObjeto.cs`**: Manual implementation of a Stack data structure (LIFO - *Last In, First Out*) using object references.
* **`playlistMusicas.cs`**: Data analytics dashboard for a music playlist using **LINQ** and Lambda expressions.
* **`FolhaDePagamento.cs`**: Payroll calculator that simulates net salary calculation with dynamic and progressive INSS and IRRF deductions.

---

## 🛠️ Project Details

### 1. Salary Average System (`MediaSalarial.cs`)

Requests the name and salary of a group of employees. It includes a validation structure to prevent the insertion of values below the established minimum salary (R$ 1,400.00). At the end, the program calculates the group average and displays which employees earn above it, while also highlighting the highest registered salary.

* **Applied concepts:** Loops (`for`, `do-while`), array manipulation, string handling, and input validation using `float.TryParse`.

### 2. Data Structure: Stack (`PilhaObjeto.cs`)

A native and dynamic implementation of a **Stack** data structure, without relying on built-in .NET collections. Each element works as a node that stores its own value and points to the next element in memory.

* **Supported operations:**

  * `Push`: Inserts a new element at the top of the stack.
  * `Pop`: Removes and returns the element at the top, with exception handling if the stack is empty.
  * `Peek`: Displays the current top value without removing it.
  * `List`: Iterates through and displays all stacked elements on the screen.

### 3. Port-A-Song Data Analytics (`playlistMusicas.cs`)

Simulates an analytics dashboard for a music catalog. The program loads a list of objects in memory and provides an interactive menu that uses **LINQ (Language Integrated Query)** to process the information.

* **Menu features:**

  1. Filter and list songs by a specific genre.
  2. Display the Top 3 most played songs based on the number of plays.
  3. Calculate the average duration, in seconds, of the entire catalog.
  4. Check whether a specific artist exists in the database through partial search.

### 4. Payroll Calculator (`FolhaDePagamento.cs`)

An interactive tool that automates employee net salary calculation by applying withholding tax rates.

* **Business rules and validations:**

  * Prevents salaries less than or equal to zero from being entered.
  * Calculates progressive INSS deductions in brackets ranging from 7.5% to 14%.
  * Applies IRRF withholding tax of 7.5% for values above the R$ 1,900.00 threshold.
  * Displays a complete statement containing the gross salary, applied deductions, and final net salary.

---

## 💻 How to Run the Projects

### Requirements

* [.NET SDK](https://dotnet.microsoft.com/download) installed on your machine.
* A code editor such as [Visual Studio Code](https://code.visualstudio.com/) or [Visual Studio](https://visualstudio.microsoft.com/).

### Step by Step

1. **Clone this repository:**

```bash
git clone https://github.com/luf3ds/C-codes.git
```
