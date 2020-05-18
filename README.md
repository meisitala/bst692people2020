# Homework 1
This is a crazy new assignment.  You will download the code for an R package that is in development, add a fuction, and publish it on github.  Then you will add some code that produces a manual page, build the documentation and publish the updated version to github. 

## Part 1
0. Install the roxygen2 package and then use it:

```
install.packages("roxygen2")
library(roxygen2)
```

1. Clone this project with R Studio
2. Add a branch with a name like rayBranch or laylaBranch or bobBranch
3. Add an R file in the R directory with a name like aboutRay.R or aboutLayla.R or aboutBob.R
4. Add a function that has some unbelievable/interesting facts and one lie about you and/or your loved ones. The function sould be like this:

```
#' @export aboutRay
aboutRay <- function() {
  cat("Which of these is a lie: \n")
  cat("1. Ray's father was the sole survivor of an airplane crash.\n")
  cat("2. Tom Cruise ran into Ray so hard at the Academy Award they both spilled their drinks.\n")
  cat("3. Ray's niece was Billie Eilish's best friend as they grew up.\n")
  cat("4. Ray's father-in-law was accused of covering up the murder of Marilyn Monroe.\n")
  cat("5. Ray took his son to the world premiere of the SpongeBob SquarePants movie in 2004.\n")
}
```
Don't forget the `#' @export line`.

Using R Studio, do the following: 

5. Speculate about what is the lie.
6. Save the file
7. Stage the file
8. Commit the file
9. Push the branch

## Part 2
1. Modify your function so it include other information needed for making the documentation

```
#' The aboutRay Function
#'
#' @description This is four truths and one lie.... The lie is xxx.
#'
#' @return NA
#' @export aboutRay
aboutRay <- function() {
  cat("Which of these is a lie: \n")
  cat("1. Ray's father was the sole survivor of an airplane crash.\n")
  cat("2. Tom Cruise ran into Ray so hard at the Academy Award they both spilled their drinks.\n")
  cat("3. Ray's niece was Billie Eilish's best friend as they grew up.\n")
  cat("4. Ray's father-in-law was accused of covering up the murder of Marilyn Monroe.\n")
  cat("5. Ray took his son to the world premiere of the SpongeBob SquarePants movie in 2004.\n")
}
```

2. Save the file
3. Use the Build menu and choose Document 
4. Check the Tab and hopefully you will see a both an R/aboutRay.R file and a man/aboutRay.Rd file
5. Commit both files
6. Push the branch
