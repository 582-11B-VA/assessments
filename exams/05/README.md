# Exam 5

> Weight: 12%\
> Due: January 5

For this exam, you must implement a function named `make-report` that
generates a report based on a given list on invoices. Each invoice has
(in order) an amount and a boolean indicating whether it has been paid.
The report must include (in order) the total amount, the total amount
paid, and the total amount due.

Please include the following tests in the `where` clause of your
function:

```pyret
make-report([list: invoice(1, true), invoice(1, false)])
  is report(2, 1, 1)
make-report([list:])
  is report(0, 0, 0)
make-report([list: invoice(10, true)])
  is report(10, 10, 0)
make-report([list: invoice(7, false)])
  is report(7, 0, 7)
make-report([list: invoice(3, true), invoice(5, true), invoice(2, true)])
  is report(10, 10, 0)
make-report([list: invoice(4, false), invoice(6, false)])
  is report(10, 0, 10)
make-report([list: invoice(0, true), invoice(0, false)])
  is report(0, 0, 0)
```

## Submission

To submit your assignment, you must first [click here][Classroom] and
follow the instructions. Once you have created the GitHub repository for
this assignment, you can use GitHub's web interface to upload your
program. Make sure to name the file "exam.arr".

[Classroom]: https://classroom.github.com/a/44hPWh8G

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
