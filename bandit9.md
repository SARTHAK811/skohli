# Bandit Level 9 to 10 Writeup
Author: [Sarthak Kohli](https://github.com/SARTHAK811) 

Problem Page: [bandit9](https://overthewire.org/wargames/bandit/bandit10.html) 

## List of Commands Used
```
ls - list files in a directory
strings - basically it grabs out human readable text in a file consisting of binary data i.e basically non text files.
grep - grep is a command that is used to search for a string of characters in a specified file.
```

## Walkthrough
How did you solve this level? Include the complete thought process, even stuff that didn't work. Give explanations wherever necessary.
To solve this level i wanted to find out few human-readable strings, preceded by several ‘=’ characters.
So intuitively it feels that i want human readable strings first and then i will see the text which is preceded by several '=' characters.
Firstly i did only strings data.txt .After doing this i got many lines of text in which i saw those text that were preceded by '=' characters.So clearly i could se that there were many lines of text that had stings of '=' in start so i used grep command so as to get only those lines that had '=' characters .Hence i used piping to do both together and got the password.

## Password
`truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk`

## Bash/Python script to automate the process
```
ssh bandit9@bandit.labs.overthewire.org -p 2220 " ls ; strings data.txt | grep '======' "
```

## Suggested modifications [Optional]
What can you do to make this level more difficult. The inherent idea should be similar.