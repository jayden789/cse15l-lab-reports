# Lab Report 3
There are a few command lines that comes in handy when working with ternimal. One of them is `find` command. \
This report will show some examples of using the `find` command that help look for files and any directories. \
* The `find` command usually has below syntax:\
\
`find [directory to search] [options] [expression]`, where\
\
`[directory to search]` is the file path for looking\
`[options]` : the type of search\
`[expression]` : the specific term of searching\
<hr>
\
* Inside the `technical` folder, there are some subfolders:\
******************** subfolder
* Inside 911report folder, there are some `.txt` files:\
*************************** chapters

## Find files by name
One way to search for a file is using `-name` option.\
For example, if we want to look for a specific file (`chapter-1.txt`) we can use:\
` find 911report/ -name "chapter-1.txt"`
************************* chapter 1
It will give the file path relative to the current directory we are working.\

`-name` is also helpful when we are looking for multiple files with given extensions. For example:\
` find 911report/ -name "*.txt"`\
It will print all the file paths containing specific term that we are looking for ( all `txt` files).

* One import thing is that `-name` will output all files **and** directories that match the specific name given\
( It will output each file path for both the file itself and directory if they both contain same specific given term)\

## Find only files
One way to find only filepath for file is telling computer specifically using `-type f` option, where `f` here means **"file"**
` find 911report/ -type f -name "chapter-1.txt"`
************************ chapter1-file
Using this command to make sure the filepath is only for file and not directory.

`find 911report/ -type f -name "*.txt"`\
***************** all-chapter-file*********
**(These file paths are paths of files instead of directory)**\

## Find multiple (specific) files 
We could find many files specifically using `-o` with `-name`\

`find ./ -name "911report" -o -name "biomed"`\
******************** using -o********** \
` find ./ -name "911report" -o -name "government"`\
******************** using -o********** \
\
## Find files with small or big size
We could search for any files that either big or small size by using `-size`\
` find ./ -size 50k `
\
------------------------ 50k -----------
\
`./` specifies the current directory so the `find` will start searching from here\
This will prints all file paths of which the file size is exactly 50KB\

` find ./ -size +1G `
---------------big size file -------------
\
`./` specifies the current directory so the `find` will start searching from here\
Clearly, there no such files that are greater than GB so nothing is printed out.\

https://linuxhandbook.com/find-command-examples/










