# Lab 1 report: Remote access and FileSystem
### Purpose:
The main purpose of this report is to instruct incoming CSE15L students how to log into a course-specific account ieng6
### Step 1: Create CSE15L account

* Look up your CSE15L account via [Account Lookup](https://sdacs.ucsd.edu/~icc/index.php), you need your **UCSD username** and **PID number**\
\
![image1](https://user-images.githubusercontent.com/112384009/230851910-003311f0-d73e-4023-8b7b-c138e7354a68.jpg)
<br><br/>
* After logging in, you need reset your password. Follow the instruction here [Reset password TUTORIALS](https://drive.google.com/file/d/17IDZn8Qq7Q0RkYMxdiIR0o6HJ3B5YqSW/view)


![image2](https://user-images.githubusercontent.com/112384009/230851912-4f571f5a-1f08-4cb7-bb34-52d13fd6283c.jpg). 


### Step 2: Install VSCode

* You can download the VSCode on the website [https://code.visualstudio.com/](https://code.visualstudio.com/).

* Choose the version that works with your OS (MAC/WINDOWNS/LINUX)

![image3](https://user-images.githubusercontent.com/112384009/230851914-981e6064-740a-4fb6-9349-0ecaca090cf5.jpg)

* Once installed, open your VSCODE

![vscode](https://user-images.githubusercontent.com/112384009/230851932-8cd8e41b-f2f8-4801-860e-86661b41d950.jpg)

(It may have different theme on your end depending on your preference)

* If you are new to VSCode, go to [https://code.visualstudio.com/docs/introvideos/basics](https://code.visualstudio.com/docs/introvideos/basics) for basic tutorials.\
![image4](https://user-images.githubusercontent.com/112384009/230851916-99f2ea5a-0f1d-4bcf-b0dd-6937891ba66d.jpg)


### Step 4: Remotely Connecting

* From your VSCode, press **Ctrl+\`** to open new terminal

![image5](https://user-images.githubusercontent.com/112384009/230851918-3d03bb5f-6741-42f1-8eda-5369155aa34e.jpg)

  * If you are using Windowns, you need to install **Git** on your computer. Go to [https://gitforwindows.org/](https://gitforwindows.org/)
  * Once installed, you can use Bash on VSCode for Windowns. You need to change to Bash command on your terminal.
* Type `ssh cs15lsp23zz@ieng6.ucsd.edu` replacing **zz** with what shown on your account to access the ieng6 server

![image6](https://user-images.githubusercontent.com/112384009/230851919-98bb53d5-1c01-458e-b477-2e9e974a73f5.jpg)

* If it's your first time access the server, it will prompt to ask your if you want to continue connecting to the server, so type `yes` to connect.
* Onced connected, your terminal will be displayed like this

![image7](https://user-images.githubusercontent.com/112384009/230851920-8ce69061-b477-4827-a426-8c578a7eb0df.jpg)

* Now you are access the remote `ieng6` server! Let try using some command lines on that server!


### Step 5: Running some commands

* There are some commands you could try: `cd`, `ls`, `pwd`, `mkdir`...
* pwd (print working directory)

![image8](https://user-images.githubusercontent.com/112384009/230851922-959b9fa8-b16c-40ea-9b13-eeb2fb70546b.jpg)

* ls (list all files in current working directory)

![image9](https://user-images.githubusercontent.com/112384009/230851924-ebb323e7-203b-4cb0-9988-80dea3c4e8df.jpg)

* Some other commands

![image10](https://user-images.githubusercontent.com/112384009/230851927-a4a69e55-9dce-41af-bcb1-ecc1ea269af6.jpg)

* To exit, type `exit` to return to your local machine

![image11](https://user-images.githubusercontent.com/112384009/230851929-e30b4e6c-ee7a-4035-9d23-382c0b42dc8f.jpg)


* Now you are back to your local machine. Try typing these command on your local machine to see what's gonna happen!
