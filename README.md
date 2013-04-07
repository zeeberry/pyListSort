pyListSort
==========

List sorting in Python. 

The Problem

Write a program that takes a list of strings containing integers and words and returns a
sorted version of the list.

The goal is to sort this list in such a way that all words are in alphabetical order and all integers
are in numerical order. Furthermore, if the nth element in the list is an integer it must remain an
integer, and if it is a word it must remain a word.

In addition, the strings and integers may contain characters that are ascii symbols that neither
belong to letter set nor digit set (i.e. "#", "%", ";", etc). You are required to remove them during the
process so that the output will contain only letters or digits. For example, if a string is "sym*bo+l",
the output should be "symbol". If an integer is "12%3", the output should be "123".

You don't have to worry about handling the following case:
Strings or integers that contain only non-letter-non-digit characters, like "^!?", "&", etc. We will not
test your program with this.

I/O

The input will be a file includes a single, possibly empty, line containing a space-separated list of
strings to be sorted. Words will not contain spaces, will contain upper-case, lower-case letters a-
z and maybe non-letter-non-digit characters. Integers will be in the range -999999 to 999999, and
might also contain non-letter-non-digit characters.

The program must be printed into a file named "result.txt". The content of the file is the list of
strings, sorted per the requirements above. Strings must be separated by a single space, with no
leading space at the beginning of the line or trailing space at the end of the line.

The program should take the input file name as the first argument, output file as the second
argument:

root:# ./listSorting.py <path-to-input-file>/list.txt <path-to-output-file>/result.txt
