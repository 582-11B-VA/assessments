# Exam 4

> Weight: 12%\
> Due: December 19

For this exam, you must implement two functions that operate on hands of
playing cards. In this program, a hand is represented as a list of
cards, where each card is a string in the format "RANK-SUIT". For
example:

- "10-H" represents the 10 of hearts,
- "A-S" represents the ace of spades,
- "3-D" represents the 3 of diamonds,
- "K-C" represents the king of clubs.

The first function, named `is-same-suit`, determines whether all the
cards in a given hand are of the same given suit. The following tests
must be included with your function:

```pyret
is-same-suit([list: "10-H", "J-H"], "H") is true
is-same-suit([list: "10-H", "J-D"], "D") is false
is-same-suit([list: "A-S", "9-S", "Q-S"], "C") is false
is-same-suit([list: "3-S"], "S") is true
```

The second function, named `to-ranks`, returns the cards in a given hand
but without the suit. The following tests must be included with your
function:

```pyret
to-ranks([list: "10-H", "J-H"]) is [list: "10", "J"]
to-ranks([list: "10-H", "J-D"]) is  [list: "10", "J"]
to-ranks([list: "A-S", "9-S", "Q-S"]) is  [list: "A", "9", "Q"]
to-ranks([list: "3-S"]) is [list: "3"]
```

## Submission

To submit your assignment, you must first [click here][Classroom] and
follow the instructions. Once you have created the GitHub repository for
this assignment, you can use GitHub's web interface to upload your
program. Make sure to name the file "exam.arr".

[Classroom]: https://classroom.github.com/a/tadj-HCH

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
