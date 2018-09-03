---
title: 'Getting Started'
description: 'This chapter provides some basic information for working with R and with DataCamp.'
---

## The R Console

```yaml
type: NormalExercise 
lang: r
xp: 100 
skills: 1
key: e127597aa1   
```


The R CONSOLE at the lower right is just like the R prompt you see when you start R (or RStudio) on your own computer. You can execute R commands (like 3 + 4) straight in the console. This is a good way to experiment.


`@instructions`
- Type 3 + 4 in the console and then hit return.
- Type 3 + 4 in the SCRIPT.R window in the upper right (next to the "3") and then hit Submit Answer

`@hint`
All I am looking for is that you type:
3 + 4
in the SCRIPT.R window in the upper right, next to the "3".

`@sample_code`

```{r}
# This window, titled SCRIPT.R, is the place to type in your answers.
# The hash sign (#) indicates that what follows is a comment, which R will ignore.
```


`@solution`

```{r}
3 + 4
```


`@sct`

```{r}
test_error()
test_output_contains(3 + 4)
test_student_typed("3 + 4", not_typed_msg = "Something is wrong with your answer. Take another look at the instruction.")
success_msg("Excellent! See how the console shows the result of the R code you submitted?")
```


---

## How DataCamp works

```yaml
type: NormalExercise 
lang: r
xp: 100 
skills: 1
key: 461f3c4158   
```


Type R code to solve the exercises into the SCRIPT.R window on the upper right. Click on the 'Run Code' buttom to cause R to interpret and execute your code. This is a good way of trying out your answer before you formally submit it. The output of your R code is shown in the console in the lower right corner. R makes use of the # sign to add comments, so that you and others can understand what the R code is about. Comments are not run as R code, so they will not influence your result. For example, "# Calculate 3 + 4" in the editor on the right is a comment.

Once you think your code is correct, hit the 'Submit Answer' button. DataCamp will evaluate your answer.


`@instructions`
- In the editor on the right there is already some sample code. Can you see which lines are actual R code and which are comments?
- Add a line of code that calculates the sum of 9 and 3, and hit the 'Submit Answer' button.

`@hint`
All I am looking for is that you type:
9 + 3
in the SCRIPT.R window in the upper right, next to the "5" and then hit "Submit Answer."

`@sample_code`

```{r}
# Calculate 3 + 4
3 + 4

# Calculate 9 + 3
```


`@solution`

```{r}
9 + 3
```


`@sct`

```{r}
test_error()
test_output_contains(9 + 3)
test_student_typed("9 + 3", not_typed_msg = "Something is wrong with your answer. Take another look at the instruction.")
success_msg("Excellent! See how the console shows the result of the R code you submitted?")
```


---

## R as a calculator

```yaml
type: NormalExercise 
lang: r
xp: 100 
skills: 1
key: a9b6211ed4   
```


In its most basic form, R can be used as a simple calculator. Consider the following arithmetic operators:

    Addition: +
    Subtraction: -
    Multiplication: *

With this knowledge, follow the instructions below to complete the exercise.


`@instructions`
- Type 5 - 2 in the editor to calculate the difference between 5 and 2.
- Type 3 * 4 in the editor to calculate the product of 3 and 4.

Note you can experiment directly in the console. You can also try "Run Code" before you submit your answer. Click 'Submit Answer' and have a look at the R output in the console. Note how the # symbol is used to add comments on the R code.

`@hint`
All I am looking for is that you type:
5 - 2
3 * 4

`@sample_code`

```{r}
# An addition
5 + 5 

# A subtraction


# A multiplication
```


`@solution`

```{r}
5 - 2
3 * 4
```


`@sct`

```{r}
test_error()
test_output_contains(5 - 2)
test_output_contains(3 * 4)
success_msg("Excellent!")
```


---

## Use a function

```yaml
type: NormalExercise 
lang: r
xp: 100 
skills: 1
key: 17f0b66368   
```


R has thousands of built in functions for calculating quantities and performing actions. You "call" a function by typing its name. All functions are ended with parantheses. sqrt is the name of the function which calculates a square root, but to call the function we need to include parantheses at the end. Many functions take "arguments," which are provided within the parantheses.


`@instructions`
- Calculate the square root of 4.

`@hint`
All I am looking for is that you type:
sqrt(4)
in the SCRIPT.R window in the upper right, next to the "5" and then hit "Submit Answer."
Very soon, these hints will be less explicit!

`@sample_code`

```{r}
# Calculate the square root of 9
sqrt(9)

# Calculate the square root of 4
```


`@solution`

```{r}
sqrt(4)
```


`@sct`

```{r}
test_error()
test_student_typed("sqrt(4)", not_typed_msg = "Something is wrong with your answer. Take another look at the instruction.")
success_msg("Excellent!")
```


---

## Create a variable x and make it equal 4

```yaml
type: NormalExercise 
xp: 100 
key: 3761ff0384   
```


You can also create variables, something which can contain specific values. We use the assignment operator (<-) for this purpose.  It is a less-than sign (<) followed by a dash (-).


`@instructions`
- Assign the value 4 to the variable x with the assignment operator.

`@hint`
If you really need a hint for this question, this course may be too tough for you!

`@sample_code`

```{r}
# The below code assigns the value 3 to the variable y
y <- 3
# Type below the code which assigns the value 4 to the variable x
```


`@solution`

```{r}
x <- 4
```


`@sct`

```{r}
test_error()
test_student_typed("x <- 4", not_typed_msg = "Something is wrong with your answer. Take another look at the instruction.")
success_msg("Excellent!")
```


---

## Load a package

```yaml
type: NormalExercise 
xp: 100 
key: e79c98eec9   
```


Although R starts with many functions, like addition, enabled by default, we need to explicitly load others ourselves. R organizes its functions into _packages_.  To use a package, you must first _install_ it and, second, _load_ it.

- You install packages using the install.packages() command.
- You load a package with the library() command.

When using DataCamp, you never need to install a package. All the packages you need are already installed on our servers. Also, in general, you do not need to load a package since doing so repeatedly would get very annoying. Instead, I will explicitly tell you to load a library in certain exercises, like this one.


`@instructions`
Load the ggplot2 package with the library() command

`@hint`
library(ggplot2) is all you need. In fact, it is already there!
Just hit "Submit Answer"

`@sample_code`

```{r}
# Load package below
library(ggplot2)
```


`@solution`

```{r}
library(ggplot2)
```


`@sct`

```{r}
success_msg("Excellent!")
```


