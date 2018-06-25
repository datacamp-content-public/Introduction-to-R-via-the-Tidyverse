---
  title: "Getting Started"
  description: "This chapter provides some basic information for working with R."
  v2: true

---
## How DataCamp works

```yaml
type: NormalExercise
lang: r
xp: 100
skills: 1
key: e127597aa1



```

In the editor on the right you should type R code to solve the exercises. When you hit the 'Submit Answer' button, every line of code is interpreted and executed by R and you get a message whether or not your code was correct. The output of your R code is shown in the console in the lower right corner.

R makes use of the # sign to add comments, so that you and others can understand what the R code is about. Just like Twitter! Comments are not run as R code, so they will not influence your result. For example, Calculate 3 + 4 in the editor on the right is a comment.

You can also execute R commands straight in the console. This is a good way to experiment with R code, as your submission is not checked for correctness.

`@instructions`
-In the editor on the right there is already some sample code. Can you see which lines are actual R code and which are comments?-
Add a line of code that calculates the sum of 6 and 12, and hit the 'Submit Answer' button.

`@hint`
- Just add a line of R code that calculates the sum of 6 and 12, just like the example in the sample code!


`@sample_code`
```{r}
# Calculate 3 + 4
3 + 4

# Calculate 6 + 12
```
`@solution`
```{r}
2 + 2
```
`@sct`
```{r}
# Update this to something more informative.
success_msg("Awesome! See how the console shows the result of the R code you submitted? Now that you're familiar with the interface, let's get down to R business!")
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
Assign the value 4 to the variable x with the assignment operator.

`@hint`
x <- 4



`@solution`
```{r}
x <- 4
```
`@sct`
```{r}
x == 4
```






---
## Load the Tidyverse

```yaml
type: NormalExercise

xp: 100

key: e79c98eec9



```

Although R starts with many functions, like addition, enabled by default, we need to explicitly load others ourselves. R organizes its functions into packages. You load packages with the library() command.

`@instructions`
Load the tidverse package with the library() command

`@hint`
library(tidyverse)

`@pre_exercise_code`
```{r}
library(tidyverse)
```

`@solution`
```{r}
library(tidyverse)
```
`@sct`
```{r}
"tidyverse" %in% .packages()
```






---
## Insert exercise title here

```yaml
type: NormalExercise

xp: 100

key: a9b6211ed4



```

In its most basic form, R can be used as a simple calculator. Consider the following arithmetic operators:

    Addition: +
    Subtraction: -
    Multiplication: *
    Division: /
    Exponentiation: ^
    Modulo: %%

The last two might need some explaining:

    The ^ operator raises the number to its left to the power of the number to its right: for example 3^2 is 9.
    The modulo returns the remainder of the division of the number to the left by the number on its right, for example 5 modulo 3 or 5 %% 3 is 2.

With this knowledge, follow the instructions below to complete the exercise.

`@instructions`
- Type 2^5 in the editor to calculate 2 to the power 5.
    - Type 28 %% 6 to calculate 28 modulo 6.
    - Click 'Submit Answer' and have a look at the R output in the console.
    - Note how the # symbol is used to add comments on the R code.

`@hint`
Another example of the modulo operator: 9 %% 2 equals 1.


`@sample_code`
```{r}
# An addition
5 + 5 

# A subtraction
5 - 5 

# A multiplication
3 * 5

 # A division
(5 + 5) / 2 

# Exponentiation
```






