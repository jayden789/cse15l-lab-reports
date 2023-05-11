# Lab Report 3
There are a few command lines that comes in handy when working with ternimal. One of them is `find` command. \
This report will show some examples of using the `find` command that help look for files and any directories.
* The `find` command usually has below syntax:\
\
`find [directory to search] [options] [expression]`, where\
\
`[directory to search]` is the file path for looking\
`[options]` : the type of search\
`[expression]` : the specific term of searching

* Inside the technical folder, there are some subfolders:
![subfolder](https://github.com/jayden789/cse15l-lab-reports/assets/112384009/a167b461-e6f4-4c82-86c3-d44454f57e17)


* Inside `911report folder`, there are some `.txt` files:\
![chapters](https://github.com/jayden789/cse15l-lab-reports/assets/112384009/98f54db1-f4fd-41e1-935d-c3b0fd0d1ff7)


## Find files by name
One way to search for a file is using `-name` option.\
For example, if we want to look for a specific file (`chapter-1.txt`) we can use:\
` find -name "chapter-1.txt"`\
\
![chapter 1](https://github.com/jayden789/cse15l-lab-reports/assets/112384009/68414c34-8aa4-44c0-8e5f-979e7114ea54)
\
It will give the file path relative to the current directory we are working.

`-name` is also helpful when we are looking for multiple files with given extensions. For example:\
` find 911report/ -name "*.txt"`

![all-txt](https://github.com/jayden789/cse15l-lab-reports/assets/112384009/98cb3d61-127a-48f6-b013-2f864c783b19)


It will print all the file paths containing specific term that we are looking for ( all `txt` files in `911report` folder).

* One import thing is that `-name` will output all files **and** directories that match the specific name given\
( It will output each file path for both the file itself and directory if they both contain same specific given term)

## Find only files
One way to find only filepath for file is telling computer specifically using `-type f` option, where `f` here means **"file"**
` find 911report/ -type f -name "chapter-1.txt"`

![chapter1-file](https://github.com/jayden789/cse15l-lab-reports/assets/112384009/d31d2878-a094-4ea6-bcb1-5b6ce410fc0b)


Using this command to make sure the filepath is only for file and not directory.

`find 911report/ -type f -name "*.txt"`


![all-chapter-files](https://github.com/jayden789/cse15l-lab-reports/assets/112384009/23b8777a-0cf8-4e82-8ee2-e065050b0c87)

**(These file paths are paths of files instead of directory)**

## Find multiple (specific) files 
We could find many files specifically using `-o` with `-name`

`find ./ -name "911report" -o -name "biomed"`


![using-o](https://github.com/jayden789/cse15l-lab-reports/assets/112384009/82c1ea03-c5f5-4bf6-b5cd-c67c0a9bf988)

` find ./ -name "911report" -o -name "government"`

![using-o2](https://github.com/jayden789/cse15l-lab-reports/assets/112384009/a917b2e7-daf5-4384-a722-8acf5eac365d)


## Find files with small or big size
We could search for any files that either big or small size by using `-size`\
` find ./ -size 50k `

![50k](https://github.com/jayden789/cse15l-lab-reports/assets/112384009/b760a0c5-5e39-4cb2-881e-2f9e815981a0)


`./` specifies the current directory so the `find` will start searching from here\
This will prints all file paths of which the file size is exactly 50KB

` find ./ -size +1G `

![big-size-file](https://github.com/jayden789/cse15l-lab-reports/assets/112384009/2984f640-ac5d-4967-bd8d-78044ef1be78)


`./` specifies the current directory so the `find` will start searching from here\
Clearly, there no such files that are greater than GB so nothing is printed out.\

Source: (https://linuxhandbook.com/find-command-examples/)










