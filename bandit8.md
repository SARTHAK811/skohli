# Bandit Level 8 to 9 Writeup
Author: [Sarthak Kohli](https://github.com/SARTHAK811) 

Problem Page: [bandit8](https://overthewire.org/wargames/bandit/bandit9.html) 

## List of Commands Used
```
ls - list files in a directory
uniq - filters out the repeated lines in a file.
sort - sort a file,arranging the recors in a particular order.
```

## Walkthrough
To solve this level I wanted to get the only line of the text that occurs only once.
so for this basically i require uniq function which filters out the repeated lines in a file .
Now in uniq function the -u option helps me to print the line that is unique.
but unique command can function only when the data is sorted. so we need to use two commands for which we have to use piping .So in piping we use multiple commands going from left to right .hence first we sort the data and then we use uniq -u command.

## Password
`UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR`

## Bash/Python script to automate the process
```
ssh bandit8@bandit.labs.overthewire.org -p 2220 "ls ; sort data.txt | uniq -u"
```
