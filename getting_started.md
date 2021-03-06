# Practical Python Week 0: Getting Started
<img width = "350" src="./images/hazel.png" align="right">

Welcome to **Practical Python**. Python is an amazing language: it is powerful, useful, ubiquitous, and relatively easy to learn -- even for people with no programming experience. For this background class we will focus mainly on setting up your programming environment.

Note if you are already comfortable with Conda and Jupyter, you can skip  to Step 3: _Download repo and run test notebook_.

Getting a programming environment set up that will work without any hiccups is essential. With Python, this step can sometimes be daunting because there are so many options -- unlike  Matlab, which has a single interface, Python has at least a dozen to choose from. Hence, to avoid confusion and be sure we are all on the same page, our first task will be to set up and test drive one popular programming environment for scientific computing.

We are going to be using anaconda (technically, a streamlined version of anaconda called *miniconda*), and Jupyter. Jupyter notebooks have become the *de facto* standard that scientists and data scientists use to communicate with one another in Python.

Please be sure to set aside a good chunk of time for this initial step, as it isn't just about installation, but about practicing how to start and use Jupyter notebooks, among other things. Also, there is a slight chance you will end up in install hell, and it will be crucial to escape well before our first real class, which will be focused on Python itself rather than installation issues.

# 1. Install and test Python
## Install miniconda
We will be installing Python version 3.8, following the directions below. Installation will probably go smoothly and quickly, but if you run into snags (especially mac users), Google is your friend. There are lots of great online resources like [Stack Overflow](https://stackoverflow.com/) where people post their solutions to problems.

*Windows users*
1. Go to the download page:https://docs.conda.io/en/latest/miniconda.html and download the installer for Python 3.8 (`Miniconda3-latest-Windows-x86_64.exe`).
2. Once downloaded, click on the executable and accept all the default settings
3. If you get stuck, this youtube video is good: https://www.youtube.com/watch?app=desktop&v=XCvgyvBFjyM

*Mac users*    
Basically, follow this video:    
https://www.youtube.com/watch?v=2kNj5oBpfyY

1. Go to the download page:https://docs.conda.io/en/latest/miniconda.html and download the package installer for Python 3.8 (`Miniconda3-latest-MacOSX-x86_64.pkg`).
2. Once downloaded, click on the package file and accept all the default settings (e.g., install for me only, allow to access downloads folder).
3. Open your Mac Terminal application, go to your home directory (go home using the `cd ~` command). If conda is activated, you will see the word `(base)` before your terminal prompt. Go to step 5. If not, then go to step 4.
4.  Enter the following commands in your terminal:
```
    cd ~    
    bash        
    source .bash_profile    
    conda init zsh    
```
Close the terminal, open new one, and go to step 5.
5. You should see the word `(base)` in front of your terminal prompt, which means anaconda was installed. Type in the following just to test it:
```
conda list
```
If you see a list of stuff, then it worked, congrats! If not, try closing your terminal and starting it again.


## Test Python
1. First, open your Anaconda terminal:
- In Windows, click your Windows button and search `Anaconda` and you will see `Anaconda Prompt` click on it, and you will open a special Anaconda terminal. Right click to pin it to your taskbar because you will be using this all the time.
- On the Mac, just open your Terminal app as before.
2. In the terminal, type in the word `python`. Your prompt should change to the python prompt `>>>`
3. In your new Python terminal, enter    
    `print(???hello world!???)`    
    You should see the phrase "hello world!" echoed back to you in the terminal. If so, congrats, you have just executed your first Python program!
4. Write `exit()` into your terminal (be sure to include parentheses), and it will bring you back to your original terminal. Close your terminal.

Congratulations! If everything worked, you are ready to become a Pythonista! You could actually start writing Python code in your terminal. However, thaw would quickly become very tedious, so let's install Jupyter next, so you can have a more pleasant programming experience.

# 2. Install and test Jupyter
When you installed anaconda, you weren???t just installing Python. Conda is a powerful tool for managing and installing Python packages -- it is used by pretty much everyone who does data analysis in Python. We will use it for all sorts of things in the class, starting with Jupyter.

## Install Jupyter (and git)
Let's go back to your Anaconda prompt (Windows) or your terminal (Mac). Enter the following commands:

    conda install -c conda-forge notebook
    conda install -c anaconda git

As usual when installing packages, you will be prompted about whether you are sure you want to proceed: say yes (`y`). You have just installed Jupyter, our main programming environment (which you will learn a lot more about soon), and *git* (a version control system that we will use to download course content).

## Hello, Jupyter: create a notebook
1. Create a folder for all your class stuff, go into that folder, and start your Jupyter notebook server. Note in general when using anaconda we will use many common  terminal commands for moving around and making new directories (`cd` for 'change directory' and `mkdir` for 'make directory'):
- On the mac, in the terminal:
```
    cd ~
    mkdir learning_python
    cd learning_python
    jupyter notebook
```
- In Windows in the Anaconda prompt:
```
    mkdir learning_python
    cd learning_python
    jupyter notebook
```
You will be doing those last two terminal commands very frequently during this class. That is:
```
cd learning_python
jupyter notebook
```
is how you will launch your programming environment and start your Jupyter server, so you probably will want to get used to doing this.

2. The above commands should start your Jupyter server, and open up your Jupyter home page in your browser. It will look like the image below (don't worry about the details -- for now just make sure it opened):

<img src="./images/jupyter_server_home.jpg" align="center">        


3.  Click on the `New` dropdown menu (circled in red in the image above) and click on `Python 3` to open up your first Jupyter notebook. It will look like the image below. The notebook name (circled in cyan) will be  `Untitled` at first: you can click on the title field and name it something else like `test_notebook`. The other labeled parts of the notebook (Menu, Toolbar, Cell) will all be discussed later.    

<img src="./images/jupyter_notebook_blank.jpg" align="center">

4. Let's give the notebook a very quick test-drive. Double-click into the empty cell (highlighted in blue in the image above), type in `1+1` and then `shift-Enter` to run the code. You should then see the number `2` printed out below the cell, and a new cell will be created.

6. Save your work (click on the save icon in the toolbar, or `ctrl-s`). If all of the above worked, congratulations, you have successfully set up your Python programming environment! You can safely close your Jupyter tabs and hit `ctrl-c` in your terminal to terminate the Jupyter server.

Now that we everything is set up, we can actually start the class properly.

# 3. Download repo and run test notebook
Our first step is to download the content of the class from github. In your terminal, go to the folder you made for the class:

    cd learning_python
    git clone https://github.com/EricThomson/practical_python
    cd practical_python
    jupyter notebook

What we have done is cloned the course content from git into directory called `practical_python`, entered that directory, and launched the Jupyter server from there.  

In the server home page you will see lots of notebooks for different weeks. For now, click on  `week0.ipynb`. This notebook contains the main lesson for your first week: it includes some basic background about programming, Python, Jupyter notebooks, and gives you a chance to practice entering stuff in Jupyter.

# 4. Celebrate!
If you have made it through the steps above, then pat yourself on the back and take a break.  You are well on your way to using Python for cool data analysis, visualization, and machine learning applications. Most importantly, you are ready for our first actual class. You have parked your car facing downhill, ready to release the parking break and move fast and break things!
