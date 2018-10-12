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
1. Ask a question that requires a student to understand the difference between accessing a column in a matrix with text indices versus accessing a column in a data frame with text indices. Your question should require an answer comparing the following: mymatrix[,'col1'] vs. mydf[,'col1'] vs. mydf['col1'] vs. mydf$col1 vs. mydf[['col1']].
1. Ask a question that requires a student to understand the difference between accessing a column in a matrix with numeric indices versus accessing a column in a data frame with numeric indices. Your question should require an answer comparing the following: mymatrix[,1] vs. mydf[,1] vs. mydf[1] vs. mydf[[1]].

Response:

Explanation:

Script:


### Question 3

Prompt 2: Ask a question that requires a student to understand how to create a simple script and make it usable by everyone, but only writeable by its creator. Your question should require an answer using chmod NNN (using octal permissions).

-*Hint 1:* in order for a script to be executable, it must be readable and executable
-*Hint 2:* in order for a script to be executable, all of its parent directories must be executable

Response:

Script:
