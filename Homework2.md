# EE282 Homework 2 
## October 15, 2018

### Question 1
Prompt 1: Ask a question that requires a student to understand basic manipulation of files. Your question should require an answer using at least the following commands/concepts: ls, touch, mv, rm

Response: Log onto the HPC into your class directory. See all the files in the folder of your name. Make a file named "testing". Confirm that "testing" file was made. Change the name of "testing" to "awesomeness". Confirm the name change has been made. Remove "awesomeness"

Script:

```sh
$ pwd
$ cd /pub/jje/ee282/${USER}
$ ls
$ touch testing
$ ls
$ mv testing awesomeness
$ ls
$ rm awesomeness
```

### Question 2
Prompt
1. Ask a question that requires a student to understand the difference between accessing a column in a matrix with numeric indices versus accessing a column in a data frame with numeric indices. Your question should require an answer comparing the following: mymatrix[,1] vs. mydf[,1] vs. mydf[1] vs. mydf[[1]].

Response: In R, make a simple matrix and a simple dataframe. What is the difference between accessing a column in a matrix with numeric indices and accessing a column in a data frame with numeric indices? Compare the following outputs of: mymatrix[,1] vs. mydf[,1] vs. mydf[1] vs. mydf[[1]].

Explanation: In general, matrices can only store one type of data within the entire matrix, whereas data frames can store multiple types of data within each column. In other words, data frames are designed to store heterogenous vectors while matrices are not. Therefore, your output when you access a column in a matrix, will be of a uniform data type, while that might not be the case for the data frame.
  The output of mymatrix[,1] is a vector containing the matrix values in column one. Similar to mymatrix[,1], mydf[,1] also yields a vector with the values of column 1 in the data frame. The mydf[1] output for the data frame is the first actual column output in column form, not a vector containing the values within the column. The double brackets from mydf[[1]] allows for subsetting the dataframe by column name and also by index number. Thus, mydf[[1]] and mydf[['col1']] yield the same output. The mydf[[1]] output is similar to mydf[,1] in that it extracts the vector that makes up column 1. 

Script:

```sh
mymatrix <- matrix(data = 1:12, nrow = 3, ncol = 4)
mymatrix

mymatrix[,1]

mydf <- data.frame(col1 = 1:12, col2 = 3, col3 = 4)
mydf

mydf[,1]

mydf[1]

mydf[[1]]

mydf[['col1']]

```


### Question 3

Prompt 2: Ask a question that requires a student to understand how to create a simple script and make it usable by everyone, but only writeable by its creator. Your question should require an answer using chmod NNN (using octal permissions).

-*Hint 1:* in order for a script to be executable, it must be readable and executable
-*Hint 2:* in order for a script to be executable, all of its parent directories must be executable

Response:

Script: