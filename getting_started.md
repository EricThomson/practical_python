# Practial Python Week 0: Getting Started
<img width = "300" src="./images/green_python.png" align="right">

Python is an amazing language: it is powerful, useful, ubiquitous, and relatively easy to learn -- even for beginners.

Unfortunately, one of the toughest steps is getting your programming environment set up properly because there are so many options (unlike,  Matlab, which has a single convenient development environment, Python has at least a dozen to choose from). The initial setup is often harder than programming itself, so before we even meet for the first class it’s crucial to have things set up so everyone in the class is on the same page.

For Python, we are going to be using anaconda (technically, a streamlined version of anaconda called *miniconda*), and for programming we will be using Jupyter notebooks, which have become the standard tool that Python programmers use these days for communicating code to each other.

Before we meet, please run the steps below. They will install miniconda and Jupyter, and give them both a test run to make sure everything is working properly. You will also download and run a test notebook as well as our first class. This will let us spend our first class entirely on coding rather than “My Python is broken.”

#### A sidebar on install hell
<img width = "150" src="./images/this_is_fine.jpg" align="right">

Note in preparing for this class you are going to be doing a lot of steps like "install this and test it; now install that other thing and test it." Unfortunately getting your environment set up and working is a necessary rite of passage with every programming language. It is also something I would not put off until the last minute: if the following steps go *very smoothly*, I would expect it to take a conscientious beginner a few hours. However, if you end up in install hell, it could take longer, so please plan accordingly. Also bear in mind that install hell is something that everyone goes through, no matter how smart or talented they are. Because of C++, and the pre-anaconda days of Python, I have probably spent at least a month of my life in install hell. Google is your friend: millions of people have installed the following software packages; if you run into a problem, someone else has also run into it, figured out what to do, and ranted about it online with a solution.

# Install and test Python
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

# Install and test Jupyter
When you installed anaconda, you weren’t just installing Python. Conda is a powerful tool for managing and installing Python packages -- it is used by everyone who does data analysis in Python. We will use it for all sorts of things in the class, starting with Jupyter.

## Install Jupyter
Let's go back to your Anaconda prompt (Windows) or your terminal (Mac). We will now install Jupyter so we can use Jupyter notebooks. Enter the following command:

    conda install jupyter git

You will be prompted about whether you are sure you want to proceed: type in yes (`y`). Here we are installing two things: `Jupyter` and `git`. Git is a version control system that will let you download a clone of this course that I’ve uploaded to GitHub (GitHub is a code repository system used by most software developers, and you don't need to worry about that right now).

## Test Jupyter
Just have them open a new notebook and run 1+1 shift-Enter and make sure it works for now and that’s it!

Pick a folder in your computer where you are going to want to put a folder for the class. This is sort of important, because this will be your home base for the next four weeks: whenever you run Jupyter, it is going to be from here. Make sure it is convenient to reach using the cd command as you will be going there a lot over the next few weeks. Create a `learning_python` directory and cd into that folder from your Anaconda Prompt (Windows) or terminal (mac).

(this directory will have practical_python repo, as well as their personal stuff, all in one place).

Since Jupyter is a browser-based programming tool, make sure you have a browser open (typically it works well with Firefox by default, but you might need to play around), and enter the command jupyter notebook in your terminal.

SCREENSHOTS all the things.

Learn something about Jupyter?

https://realpython.com/jupyter-notebook-introduction/

Notebook Basics is realllllly good.
https://github.com/ipython/ipython-in-depth/blob/7e5ce96cc9251083979efdfc393425f1229a4a68/examples/Notebook/Notebook%20Basics.ipynb

#  Download and run a test notebook
git clone?
E. make a folder where you want all your shit.
F. Go in there open

Create jupyter notebook and add a couple of videos for them to watch.

https://github.com/flatironinstitute/mfa_jupyter_for_programming


# Now what?
Take a break, drink some tea or sparkling something. If you have done all of the above steps, congratulations! This is a pretty major accomplishment.

If you can do the above, before even meeting for the first class, then I guarantee you can use Python to run cool data analysis, visualization, and machine learning applications. Because that was a lot of work, and installation is probably the **least fun** part of learning Python.

Now you are ready for our first actual class, we are all parked facing downhill and ready to learn!

Open up the class 1 jupyter notebook, read it first or not, and that’s what we will be going over in our first class!
