# minicppproject1 — Student Marks Analyzer

A small command-line C++ program that reads the marks of a group of students and prints a summary report.

## Features

- Enter marks for 1 to 100 students
- Calculates:
  - Total marks
  - Average mark
  - Highest mark
  - Lowest mark
  - Number of students who passed (mark ≥ 40) and failed
- Run the analysis again without restarting the program

## Requirements

- A C++ compiler such as `g++` or `clang++` (C++11 or newer)

## Build and run

```bash
g++ -std=c++17 -Wall program.cpp -o program
./program
```

On Windows (MinGW):

```bash
g++ program.cpp -o program.exe
program.exe
```

## Example

```
============================
   STUDENT MARKS ANALYZER
============================
Enter number of students: 3
Enter mark of student 1: 50
Enter mark of student 2: 30
Enter mark of student 3: 90

========== STUDENT REPORT ==========
Total Marks  : 170
Average      : 56.6667
Highest Mark : 90
Lowest Mark  : 30
Passed       : 2
Failed       : 1
====================================

Do you want to analyze again? (y/n): n

Thank you for using Student Marks Analyzer!
```

## Program structure

| Function        | Purpose                                         |
|-----------------|-------------------------------------------------|
| `readMarks`     | Reads each student's mark from the keyboard     |
| `findTotal`     | Adds up all marks                               |
| `findAverage`   | Returns the average mark                        |
| `findHighest`   | Returns the highest mark                        |
| `findLowest`    | Returns the lowest mark                         |
| `countPassed`   | Counts students with a mark of 40 or more       |
| `printReport`   | Prints the summary report                       |
| `main`          | Shows the menu and repeats until the user quits |

## Notes

- The pass mark is fixed at **40**.
- Enter whole numbers only. Typing letters where a number is expected is not handled yet.
