# Practial Python Week 0: Getting Started
<img width = "300" src="./images/green_python.png" align="right">

Python is an amazing language: it is powerful, useful, ubiquitous, and relatively easy to learn -- even for beginners.

One of the most important steps is getting your programming environment set up. This can sometimes be daunting because there are so many options. Unlike with Matlab, which has a single convenient development environment, Python has at least a dozen to choose from. Before we meet for the first class everyone should set themselves up with a programming environment. This is a serious lesson in its own right, with lots of moving parts, so I would recommend that you set aside a good chunk of time for it.

We are going to be using anaconda (technically, a streamlined version of anaconda called *miniconda*), and for entering code we will be using Jupyter notebooks. Jupyter notebooks have become the *de facto* standard that Python programmers use these days for communicating with one another.

The steps below will install miniconda and Jupyter, and give them both a test run to make sure everything is working properly. You will also download and run a test notebook, and the notebook that contains our first class. All this preparation will let us spend our first class entirely on coding rather than “My Python is broken” (for more on the half-flipped teaching philosophy I'm following see [LINK HERE]).

#### A sidebar on install hell
<img width = "150" src="./images/this_is_fine.jpg" align="right">

Note for this class you are going to be doing a lot of steps like "install this and test it; now install that other thing and test *it*." This is an important rite of passage with every programming language, and if the following steps go *very smoothly*, I would expect it to take a conscientious beginner about [[FOUR]] hours. However, if you end up in install hell, it could take longer, so please plan accordingly. Also bear in mind that install hell is something that everyone goes through: it is not an indication that "Programming isn't for me". I love programming, and because of C++, and the pre-anaconda days of Python, I have probably spent at least a month of my life in install hell. Google is your friend: millions of people have installed the following software packages; if you run into a problem, someone else has also run into it, figured out what to do, and ranted about it online with a solution. I am also here to help.

# 1. Install and test Python
## Install miniconda (Python)
First, download the version of miniconda appropriate for your OS:
https://docs.conda.io/en/latest/miniconda.html

Install Python version 3.8 (64 bit), following the directions below. Installation will probably go smoothly and quickly, but if you run into snags, Google is your friend. There are lots of great resources, both videos and web sites, from folks who have been through install hell who want to help. If you remain stuck, contact me on Slack.

*Windows users*

1. Download and click on the executable (Miniconda3-latest-Windows-x86_64.exe).
2. During installation, under Advanced Options it will ask if you want to add Anaconda to your Path environment variable.  Click yes (it will tell you it is not recommended, but do it as it will make your life much easier). Also leave the other option clicked (‘Register Miniconda as my default Python’).

*Mac users*

1. Download the file to your Downloads folder (Miniconda3-latest-MacOSX-x86_64.sh)
2. Open a terminal and go to your Downloads folder (cd Downloads), and install miniconda with `bash Miniconda3-latest-MacOSX-x86_64.sh`. You will probably need to press the space bar a bunch of times to scroll through some stuff, and then ‘y’ or ‘yes’ to accept the miniconda license. Close your terminal.

You should now have conda (and therefore Python) installed on your system! Let’s test this out. The way it works is that there will be an Anaconda prompt you can open, and from there the magic happens. Let’s test it out.

## Test Python
1. First, open your conda terminal:
- In Windows, click your Windows button and search `Anaconda` and you will see `Anaconda Prompt` click on it, and you will open a special Anaconda terminal. Right click to pin it to your taskbar because you will be using this all the time.
- On the Mac, just open a terminal it is already a conda terminal because Macs are pretty much built for developers.

2. Once the conda terminal is open, type in the word `python`. This should change things – you should have opened up Python and see a new Python terminal (your prompt will now be `>>>`)!
3. In your new Python terminal, enter    
    `print(“hello world!”)`

4. Congrats! You have written some Python code! Now write `exit()` into your terminal (be sure to include parentheses), and it will bring you back to your system terminal. Close your terminal.

There you have it, if everything worked you are ready to become a Pythonista! But you don’t want to code at the terminal it would quickly become very tedious. Let’s install Jupyter next, so you can have a more pleasant programming experience.

# 2. Install and test Jupyter
When you installed anaconda, you weren’t just installing Python. Conda is a powerful tool for managing and installing Python packages -- it is used by everyone who does data analysis in Python. We will use it for all sorts of things in the class, starting with Jupyter.

## Install Jupyter
Let's go back to your Anaconda prompt (Windows) or your terminal (Mac). We will now install Jupyter so we can use Jupyter notebooks. Enter the following command:

    conda install jupyter git

You will be prompted about whether you are sure you want to proceed: type in yes (`y`). Here we are installing two things: `Jupyter` and `git`. Git is a version control system that will let you download a clone of this course that I’ve uploaded to GitHub (GitHub is a code repository system used by most software developers, and you don't need to worry about that right now).

## Test Jupyter: create and test drive Jupyter
Just have them open a new notebook and run 1+1 shift-Enter and make sure it works for now and that’s it!

Pick a folder in your computer where you are going to want to put a folder for the class. This is sort of important, because this will be your home base for the next four weeks: whenever you run Jupyter, it is going to be from here. Make sure it is convenient to reach using the cd command as you will be going there a lot over the next few weeks. Create a `learning_python` directory and cd into that folder from your Anaconda Prompt (Windows) or terminal (mac).

(this directory will have practical_python repo, as well as their personal stuff, all in one place).

Since Jupyter is a browser-based programming tool, make sure you have a browser open (typically it works well with Firefox by default, but you might need to play around), and enter the command jupyter notebook in your terminal.

SCREENSHOTS all the things.

Learn something about Jupyter?

https://realpython.com/jupyter-notebook-introduction/

Notebook Basics is realllllly good.
https://github.com/ipython/ipython-in-depth/blob/7e5ce96cc9251083979efdfc393425f1229a4a68/examples/Notebook/Notebook%20Basics.ipynb

Something about markdown, something about something.


# 3. Download and run a test notebook
git clone?
E. make a folder where you want all your shit.
F. Go in there open

Create jupyter notebook and add a couple of videos for them to watch.

https://github.com/flatironinstitute/mfa_jupyter_for_programming

Future classses will all be jupyter notebooks.


# 4. Now what?
If you have made it through the three steps above, then you definitelyl deserve a pat on the back and a break. Dance around, drink some tea or sparkling water or beer or chocolate milk. Congratulations **you have finished the hardest part of the class!** Seriously.

If you can do the above, before even meeting for the first class, then I guarantee you can use Python to run cool data analysis, visualization, and machine learning applications.

Now you are ready for our first actual class. You have parked your car facing downhill, ready to release the parking break and move fast and break things!

Open up the class 1 jupyter notebook, read it first or not, and that’s what we will be going over in our first class!
