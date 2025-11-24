# Exam 3

> Weight: 8%\
> Due: November 28

For this exam, your task is to implement a `pluralize` function that
returns the plural form of a given English word. Here are the rules your
function must follow:

1. Add "es" to words ending in "s", "x", "z", "ch", "sh".
2. Replace "y" with "ies" to words ending in a consonant plus "y".
3. Add "s" to everything else.

Your function must include and pass the following tests:

```pyret
# Rule 1
pluralize("bus") is "buses"
pluralize("box") is "boxes"
pluralize("quiz") is "quizzes"
pluralize("church") is "churches"
pluralize("brush") is "brushes"

# Rule 2
pluralize("city") is "cities"
pluralize("baby") is "babies"

# Rule 3
pluralize("cat") is "cats"
pluralize("book") is "books"
pluralize("car") is "cars"
```

## Submission

To submit your assignment, you must first [click here][Classroom] and
follow the instructions. Once you have created the GitHub repository for
this assignment, you can use GitHub's web interface to upload your
program. Make sure to name the file "exam.arr".

[Classroom]: https://classroom.github.com/a/7UCO-_Ps

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
