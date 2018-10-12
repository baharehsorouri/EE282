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

