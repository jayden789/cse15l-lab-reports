# LAB REPORT 4: RUNNING TASKS FROM COMMAND LINE (for Windown)
Firstly, log into ieng6 server from your local terminal

![login](https://github.com/jayden789/cse15l-lab-reports/assets/112384009/276059dd-1cdc-445b-9c3e-074c541e1ff1)


* Clone your fork of the repository from your Github account

Assume you did all the set up, head on your Github page and copy the repo url (either url or ssh)

![github](https://github.com/jayden789/cse15l-lab-reports/assets/112384009/f622afc7-6522-46c5-97ae-d4d7b7dd50a2)


On the terminal, type:
`git clone` then `<Ctrl-V>`. Here, `<Ctrl-V>` will paste what's been copied on the clipboard on the ternimal

![clone](https://github.com/jayden789/cse15l-lab-reports/assets/112384009/ada5eb11-2467-4cde-b15b-b32ba306ae3c)


Change direction to lab7 by typing `cd lab7/`
Here, you can use `<TAB>` to help finding the directory by typing the first character. In this case, try 
`cd l <TAB>`. It will find closest matching directory/path (We only have one directory starting at l char in current directory
so `lab7/` will be shown).

So using `<TAB>` if you don't wanna type whole path/directory/file.

Run the tests, demonstrating that they fail

In the lab7 folder, there is a bash script `test.sh`, which will test the java files\
We can run this script to test ` ListExamplesTests.java`

Tip: Using `<TAB>` for typing out file, so try:\
`bash t <TAB>`

![fail-test](https://github.com/jayden789/cse15l-lab-reports/assets/112384009/0ddcb02a-ba13-408a-95ec-8d327bb4801b)


Edit the code file to fix the failing test\
We need to fix the code for the test can be passed. One way to edit the code in `ListExamples.java` file by using Vim

So type: `vim L <TAB> .j <TAB>`

When you type L then press `<TAB>`, the terminal will not show the `ListExamples.java`, instead, it shows `ListExamples` because\
we have more than one files starting with L, and contains string `ListExamples` in the filename. So the terminal stops where\
it sees the difference, and it's up to us to choose the file we want.

![vim L](https://github.com/jayden789/cse15l-lab-reports/assets/112384009/9c4f1856-eb5b-42e6-9c3a-bee7fa9bee3d)

  
Here is  `ListExamples.java` opened on Vim
  
![notfix](https://github.com/jayden789/cse15l-lab-reports/assets/112384009/11496568-c383-439b-8407-efae41f851ab)


  
On Vim editor, make sure you are in **Normal mode**, so you can use key `k,j,h,l` for `up, down, left, right` respectively
  You can move up/down/left right with count by typing
  `<count><motion> `\
  where `<count>` is the number (how many lines/chars for moving up/down or left/right)\
  `<motion>` is one of the key `k,j,h,l` for moving the cursor
  
  You will notice the number <count> you type on the bottom right (Normal mode)
  
  ![number](https://github.com/jayden789/cse15l-lab-reports/assets/112384009/ab31dbb8-0c53-4c16-8380-e9db5bf6bea4)

  
  So try `<900><key j>` will move the cursor the the last line
  
  ![lastline](https://github.com/jayden789/cse15l-lab-reports/assets/112384009/f0c0b57f-763b-4e50-8d63-b761dd1398d4)

  
  The `<key w>` is useful for jumping to the word on current line, it will stop at the beginning of the next work\
  By combining `<count>` and `<key w>`, we can edit the code faster.
  
  So try:\
  `<2><key w><key h><key h>` will move the cursor to 1 from its position in the above picture (beginning of line)
  
  ![at1](https://github.com/jayden789/cse15l-lab-reports/assets/112384009/9d51e839-32ab-4aa5-a03b-aa1a85f116c1)

  
  #### Fixing the error
  
  `<key x><key i><2><ESC>`
  
  ![at2](https://github.com/jayden789/cse15l-lab-reports/assets/112384009/f536086b-be51-48ea-ad89-785c05ea88c7)

  
  In **Normal mode**, `<key x>` will delete the current character, so it deletes 1
  
  Then we press `<key i>` to change to **Insert mode**
  
  After fixing error, press `<ESC>` to change back to **Normal mode**\
  
  Now we save the changes and exit Vim by 
  
  `<:><key w><key q>` or `:wq`
  
  ![exit](https://github.com/jayden789/cse15l-lab-reports/assets/112384009/936cdc53-efc5-4bf7-9a49-bac337812b70)

  
  And running the test again
  
  `bash t <TAB>`
  
  ![pass](https://github.com/jayden789/cse15l-lab-reports/assets/112384009/eb114eb5-a511-4522-a001-fa7b73ef9b37)

  
  Commit and push the resulting change to your Github account
  
  Using `git add <key L><TAB> .java` , this will add file to commit stage
  
  Using `git commit -m "<Some-description>"` to commit the change\
  `"<Some-description>" is anything you wanna write
  
  ![commit](https://github.com/jayden789/cse15l-lab-reports/assets/112384009/f236574a-fd64-4cec-acc2-d08a48abba5b)

  
  If you have done with setting up SSH key, you can push to SSH key by typing
  
  `git push <Ctrl-V> main`, where `<Ctrl-V>` is the copied SSH from your Github page
  
  Copy SSH here
  
  
  ![copy](https://github.com/jayden789/cse15l-lab-reports/assets/112384009/d97af87f-20fb-4dd8-afc6-35ea75826052)

  Your repo now is pushed on the Github page
  
  ![push](https://github.com/jayden789/cse15l-lab-reports/assets/112384009/f3326b64-e26d-4475-8760-9ca14c2bb6d3)

  
  
