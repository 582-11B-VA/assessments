# Exam 2

> Weight: 8%\
> Due: November 21

For this exam, your task is to implement a function named
`minimum-ticket-price` that calculates the **minimum ticket price**
required for a movie theater's **annual revenue** to cover its
**operating costs**. When called, your function receives two arguments:

- the number of screening rooms in operation, and
- the number of days per year the theater is open.

To calculate the annual revenue, you'll first need to determine the
**number of tickets sold per year**. Each screening lasts an average of
**2 hours**. The theater is open **8 hours per day**, and each room can
accommodate **150 spectators**.

To calculate the operating costs, you must account for both **employee
wages** and **distributor fees**. Each screening room requires **2
clerks**, who are paid **\$20 per hour**. In addition, **1 supervisor**
(paid **\$25 per hour**) is required for **every 10 clerks**. E.g., 1
supervisor is needed for 5 clerks, while 2 supervisors are needed for 11
clerks. The theater must also pay an **annual licensing fee** to the
distributors, costing **\$10,000**, plus **\$200 per screening**.

Your function must include and pass the following tests:

```pyret
min-ticket-price(10, 250) is 1.94
min-ticket-price(2, 125) is 2.1
min-ticket-price(50, 200) is 1.935
min-ticket-price(5, 50) is 2
```

We strongly recommend that you break down the assignment into separate
tasks, and assign each task to a different helper function.

## Submission

To submit your assignment, you must first [click here][Classroom] and
follow the instructions. Once you have created the GitHub repository for
this assignment, you can use GitHub's web interface to upload your
program. Make sure to name the file "exam.arr".

[Classroom]: https://classroom.github.com/a/ixMpTbmy

## Assessment criteria

- Program design [5]
  - requirements are met
  - program is decomposed into functions
  - functions are assigned to a single task
  - functions are well-tested
  - common code is unified, not duplicated
  - appropriate algorithms are used, and coded cleanly

- Readability [5]
  - documentation is correct
  - constants are used instead of hard-coded values
  - complex or meaningful expressions are named
  - naming is consistent and descriptive
  - inline comments are used only to explain reasoning
  - lines are no longer than 80 characters
  - arguments are aligned vertically
  - use of whitespace is consistent
