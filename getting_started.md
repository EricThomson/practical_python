# Practical Python Week 0: Getting Started
<img width = "300" src="./images/hazel.png" style="float:right;margin:5px 5px 10px 15px">

Welcome to the first week of **Practical Python**! Python is an amazing language: it is powerful, useful, ubiquitous, and pretty easy to learn -- even if you have no programming experience. For this first class we will focus mainly on setting up and acquainting you with your programming environment.

I can understand if you are impatient to start hacking away at the nitty gritty programming bits, but getting a programming environment squared away is essential. With Python, there are *many* options. Unlike  Matlab or R, which both have a single canonical interface, Python has at least a dozen development environments to choose from. Hence, to avoid confusion, minimize choices you have to make, and be sure we are all on the same page, our first task will be to set up and test drive one popular programming environment for scientific computing.

We are going to be using anaconda (technically, a streamlined version of anaconda called *miniconda*), and Jupyter. Anaconda is a Python distribution and package manager (we will learn a lot more the details of Anaconda in Week 3), while Jupyter notebooks have become the *de facto* tool that scientists and data scientists use to write code and communicate with one another in Python.

Please be sure to set aside a good chunk of time for this initial step, as it isn't just about installation, but about practicing how to initialize and use Jupyter notebooks, building that muscle memory. Also, there is a *slight* chance you will end up in install hell, and it will be good for you to escape before our first real class.

> **Note**: if you are already comfortable with Conda and Jupyter, and have an environment set up, you can jump ahead  to Step 3 (_Download repo and run the first notebook_ -- just be sure to install git as in Step 2 if you haven't already).

# 1. Install and test Python
## Install miniconda
Let's start by installing Python. Installation will probably go smoothly and quickly, but if you run into snags (especially Mac users), Google is your friend. There are lots of great online resources like [Stack Overflow](https://stackoverflow.com/) where people post their solutions to problems. Note for users at organizations where you do not have admin on your computer: all these steps should just work, that is one of the nice things about using Conda (this is one of the things it was built for: learning Python without opening tickets with IT every five minutes). 

*Windows users*
1. Go to the download page: https://docs.conda.io/en/latest/miniconda.html and download the installer for the latest version of Miniconda (`Miniconda3-latest-Windows-x86_64.exe`).
2. Once downloaded, click on the executable and accept all the default settings
3. If you get stuck, this youtube video is good: https://www.youtube.com/watch?app=desktop&v=XCvgyvBFjyM

*Mac users*    
Basically, follow this video:    
https://www.youtube.com/watch?v=2kNj5oBpfyY

1. Go to the download page:https://docs.conda.io/en/latest/miniconda.html and download the package installer for the latest version of Miniconda (`Miniconda3-latest-MacOSX-x86_64.pkg`).
2. Once downloaded, click on the package file and accept all the default settings (e.g., Install for me only, and Allow to access downloads folder).
3. Open your Mac Terminal application, go to your home directory (enter `cd ~` at the terminal). If conda is activated, you will see the word `(base)` before your terminal prompt. If so, rejoice and go to step 5. If not, then go to step 4.    
4.  Enter the following commands in your terminal:
```
    cd ~    
    bash        
    source .bash_profile    
    conda init zsh    
```
Close your terminal, open new one, and go to step 5.    
5. You should see the word `(base)` in front of your terminal prompt, which means anaconda was installed. Type in the following in your terminal just to test it:
```
    conda list
```
If you see a list of stuff (e.g., different programs are printed out), then it worked, congrats! If not, try closing your terminal, starting a new one, and testing again.

> **Note** : in general when working from the terminal/conda prompt, there are some common terminal commands we will be using that you will want to familiarize yourself with. Mainly:
> - `cd` for 'change directory' (this will change the directory you are currently in)
> - `mkdir` for 'make directory' (this will create a new directory)
>
> If you see other commands in the terminal throughout the class and they are not explained clearly, be sure to look them up or ask your instructor what they mean. The explanation may need to be added here!

## Test Python
1. First, open your Anaconda terminal:
- In Windows, click your Windows button and search `Anaconda` and you will see `Anaconda Prompt` click on it, and you will open a special Anaconda terminal. Right click to pin it to your taskbar because you will be using this all the time.
- On the Mac, just open your Terminal app as before.
2. In the terminal, type in the word `python`. Your prompt should change to the Python terminal prompt `>>>` : this is the prompt you will see once you have Python installed and running and ready to accept commands.
3. In your new Python terminal, enter    
    `print(“hello world!”)`    
    You should see the phrase "hello world!" echoed back to you in the terminal. If so, congrats, you have just executed your first Python program!
4. Write `exit()` into the Python terminal (be sure to include parentheses), and it will bring you back to your original Anaconda terminal, which you can close.

If everything worked, you are ready to go! to the next step, congrats! You could actually start writing Python code at the terminal. However, that would quickly become pretty tedious. So let's install Jupyter next, so you can have a more pleasant programming experience.

# 2. Install and test Jupyter
When you installed anaconda, you weren’t just installing Python. Conda is a powerful tool for managing and installing Python packages -- it is used by pretty much everyone who does data analysis in Python. We will use it for all sorts of things in the class, starting with Jupyter. We will learn a lot more about conda in Week 3, but for the first couple of weeks we will just use it to learn Python.

## Install Jupyter (and git)
Let's go back to your Anaconda prompt (Windows) or your terminal (Mac). Enter the following commands:

    conda install -c conda-forge notebook
    conda install -c anaconda git

As usual when installing packages with conda, you will be prompted about whether you are sure you want to proceed: say yes (`y`). You have just installed Jupyter, our main programming environment (which you will learn a lot more about soon), and *git* (a version control system that we will use to download course content).

## Hello, Jupyter: create your first notebook
1. Create a folder to store class stuff    
 First, let's make sure we are organized for the class moving forward. We are going to want a folder for the class. Let's call it something like `learning_python`.

  Make sure you are in your terminal/anaconda prompt. 
- On the mac, in the terminal:
```
    cd ~
    mkdir learning_python
    cd learning_python
```
- In Windows in the Anaconda prompt:
```
    mkdir learning_python
    cd learning_python
```
As discussed in the note above, these commands created the directory `learning_python`, and `cd` moved us into that directory, making it our working directory.

2. Start up Jupyter  

    Once you are in the *learning_python* directory, go ahead and enter the following command in your terminal: `jupyter notebook`

    That command is how you will launch Jupyter from the terminal: get used to it, put it in your muscle memory forever.

    Once you enter that command, the Jupyter home page will open up in a new tab on your browser. It will look like the image below (don't worry about the details -- for now just make sure it opened):

<img src="./images/jupyter_server_home.jpg" style="vertical-align:middle;margin:10px 0px 30px 0px">       


3.  Create a Juypter notebook    
Click on the `New` dropdown menu (circled in red in the image above) and click on `Python 3` to open up your first Jupyter notebook. A new tab will open, your first Jupyter notebook! It will look like the image below. The notebook name (circled in cyan) will be  `Untitled` at first: you can click on the title field and name it something else like `test_notebook`. The other labeled parts of the notebook (Menu, Toolbar, Cell) will all be discussed later.    

<img src="./images/jupyter_notebook_blank.jpg" style="vertical-align:middle;margin:10px 0px 30px 0px">

4. Test it    
Let's give the notebook a very quick test-drive. Double-click into the empty cell (highlighted in blue in the image above), type in `1+1` and then `shift-Enter` to run the code. You should then see the number `2` printed out below the cell, and a new cell will be created.

5. Save your work    
Click on the save icon in the toolbar, or `ctrl-s`. If all of the above worked, congratulations, you have successfully set up your new Python programming environment! You can safely close your Jupyter tabs and hit `ctrl-c` in your terminal to terminate the Jupyter server.

Now that we everything is set up, we can actually start the class properly.

# 3. Download repo and run the first notebook
Now that you have a programming environment set up, it's about time to start! 

First, let's download the content of the class from github. In your terminal, go to the folder you made for the class if you aren't already there, and enter the following commands:

    cd learning_python
    git clone https://github.com/EricThomson/practical_python
    cd practical_python
    jupyter notebook

What we have done is entered the directory for the class that you made above, cloned the course content from git. This put all the course content into a new subdirectory called `practical_python`. We then entered that directory using `cd`, and launched Jupyter from there.  

In the Jupyter home page you will see lots of notebooks for the class. We are on Week 0, so from your Jupyter home, click on `week0.ipynb`. This notebook contains a lesson for Week 0: it includes some basic background about programming, Python, Jupyter notebooks, and gives you a chance to practice entering stuff in Jupyter.

# 4. Celebrate!
If you have made it through the steps above, then pat yourself on the back and take a break. You are well on your way to using Python for cool data analysis, visualization, and machine learning applications. Most importantly, you are ready for  class. You have parked your car facing downhill, ready to release the parking break, move fast, and break things!
