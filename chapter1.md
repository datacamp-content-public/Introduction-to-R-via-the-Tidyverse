---
  title: "Getting Started"
  description: "This chapter provides some basic information for working with R."
  v2: true

---
## Add two number at the R prompt.

```yaml
type: NormalExercise
lang: r
xp: 100
skills: 1
key: e127597aa1



```

The R programming language is a powerful and flexible tool for analyzing data. 

`@instructions`
- Add 2 and 2 together.

`@hint`
- Just type "2 + 2" (without the quotes) at the prompt and hit the "return" or "enter" key.

`@pre_exercise_code`
```{r}
# Load datasets and packages here.
```
`@sample_code`
```{r}
# Your
# sample
# code
# should
# be
# ideally
# 10 lines or less,
# with a max
# of 16 lines.
```
`@solution`
```{r}
2 + 2
```
`@sct`
```{r}
# Update this to something more informative.
success_msg("Congrats! You have started to learn R.")
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

key: 3761ff0384



```



`@instructions`


`@hint`










