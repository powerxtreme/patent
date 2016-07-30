#2. work place and files
####etwd() - *determining current working directory*

####ls() - *list all the objects in the local workplace*

####list.files() or dir() - *list all files in the local workplace*

####args() - *determining the  arguments of a funciton*

####dir.create("test") - *create a directory 'test'*

####setwd() - *set working directory*

####file.create("mytest.R") - *create a file mytest.R*

####file.exists() - *check if a file exists*

####file.info() - *access the information of a file*

####file.rename("mytest.R", "mytest2.R") - *rename file mytest.R as mytest2.R*

####file.copy("mytest2.R", "mytest3.R") - *make a copy of file mytest2.R as mytest3.R*

####file.path() - *not clear*

####dir.create(file.path("testdir2", "testdir3"), recursive = TRUE) - *directory testdir3 is a subdirectory of directory testdir2*

####unlink("testdir2", recursive = TRUE) - *delete directory testdir2, note recursive should be set to TRUE*
---
#3. Sequences of Number
1:20

pi:10

15:1

seq(1, 20)

seq(0, 10, by = 0.5)

seq(5, 10, length = 30)

my_seq <- seq(5, 10, length = 30)

rep(0, times = 40)

rep(c(0, 1, 2), times = 10)

rep(c(0, 1, 2), each = 10)

---
#4. Vectors
####`rm(list = ls())` - *clear variables in the environment*

my_char <- c("My", "name", "is")

paste(my_char, collapse = " ") - convert character vector my_char into a single character

paste(1:3, c("X", "Y", "Z"), sep = "")

---
#5. Missing Values

my_data <- sample(c(y, z), 100)

is.na(my_data)

#6. Subsetting Vectors

x[is.na(x)] - a vector of all NAs of vector x

x[!is.na(x)] - a vector of all non-NAs o vector x

***R uses `'one-based indexing'`, which (you guessed it!) means the first element of a vector is
| considered element 1.***

y[y > 0] - return a vector of all the positive elements of vector y

y[y < 0] - return a vector of all the negative elements of vector y

x[!is.na(x) & x>0] - return a vector of all the positive elements of the non-NAs of vector x

x[c(3, 5, 7)] - return a vector consisting of the third element, the fifth element and the seventh element of vector x

x[c(-2, -10)] or x[-c(2, 10)]- return a vector consisting of all the elements of vector x excluding the second element and the tenth element

vect <- c(foo = 11, bar = 2, norf = NA) - each element of vect has a name, and the element of vect can be indexed by the correspondign name

names(vect) <- list the name of the elements of vect

names(vect2) <- c("foo", "bar", "norf") - assign  names to vect2

identical(vect, vect2) - determine if two objects are sanme or not

vect[c("foo", "bar")]

---
#7. Matrices and Data Frames



