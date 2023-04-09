# Lab 1 report: Remote access and FileSystem
### Purpose:
The main purpose of this report is to instruct incoming CSE15L students how to log into a course-specific account ieng6
### Step 1: Create CSE15L account
* Look up your CSE15L account via [Account Lookup](https://sdacs.ucsd.edu/~icc/index.php), you need your **UCSD username** and **PID number**\
* After logging in, you need reset your password. Follow the instruction here [Reset password TUTORIALS](https://drive.google.com/file/d/17IDZn8Qq7Q0RkYMxdiIR0o6HJ3B5YqSW/view)
### Step 2: Install VSCode
* You can download the VSCode on the website [https://code.visualstudio.com/](https://code.visualstudio.com/)
* Choose the version that works with your OS (MAC/WINDOWNS/LINUX)\
image\
* Once installed, open your VSCODE
image
(It may have different theme on your end depending on your preference)
* If you are new to VSCode, go to [https://code.visualstudio.com/docs/introvideos/basics](https://code.visualstudio.com/docs/introvideos/basics) for basic tutorials
image
### Step 4: Remotely Connecting
* From your VSCode, press **Ctrl+\`** to open new terminal
  * If you are using Windowns, you need to install **Git** on your computer. Go to [https://gitforwindows.org/](https://gitforwindows.org/)
  * Once installed, you can use Bash on VSCode for Windowns. You need to change to Bash command on your terminal.
* Type `ssh cs15lsp23zz@ieng6.ucsd.edu` replacing **zz** with what shown on your account to access the ieng6 server
image r1
* If it's your first time access the server, it will prompt to ask your if you want to continue connecting to the server, so type `yes` to connect.
* Onced connected, your terminal will be displayed like this
image dis
* Now you are access the remote `ieng6` server! Let try using some command lines on that server!
### Step 5: Running some commands
* There are some commands you could try: `cd`, `ls`, `pwd`, `mkdir`...
* pwd (print working directory)
image pwd
* ls (list all files in current working directory)
image ls
* To exit, type `exit` to return to your local machine
image exit



