![Geekbrains Logo](https://github.com/ilyastartsdata/introductiontopython/blob/master/gb.png)

# Python libraries for Data Science

## Numpy, Matplotlib, Scikit-learn

Course from Geekbrains University

> About Geekbrains: We teach people to master programming, web design and marketing from the ground up. We conduct online courses with internships and free master classes, develop the community, cooperate with employment companies and continuously test new methods to improve the effectiveness of learning.

---

## List of topics 

**Part 1**

1. Webinar. Introduction to the course
2. Video lesson. Calculations with Numpy, working with data in Pandas
3. Webinar. Calculations with Numpy, working with data in Pandas
4. Video lesson. Visualisation of data in Matplotlib
5. Webinar. Visualisation of data in Matplotlib
6. Video lesson. Studying with a teacher at Scikit-learn
7. Webinar. Studying with a teacher at Scikit-learn
8. Video lesson. Studying without a teacher at Scikit-learn
9. Webinar. Studying without a teacher at Scikit-learn and introduction to the final project
10. Webinar. Consultation on the final project
11. Final Project

**Part 2**

1. Webinar. Introduction to the classification task, task definition and data preparation
2. Webinar. Data analysis and statistical hypothesis testing
3. Webinar. Building a classification model
4. Webinar. Evaluation and interpretation of the model obtained, discussion of the course project

---

## Installing / Getting started

### Getting started with Jupyter Notebook

Python programmes can be launched in two main ways.

1. You can write the whole programme, save it in a file or several files and then run the whole programme and get the result of its work

2. An interactive console can be started and commands entered one by one, resulting in the execution of each command separately

In Data Science, the second option tends to be more convenient, since working with data is usually a research job. It is not always aimed at writing a specific programme.

The usual interactive console has a very convenient analogue - Jupyter Notebook. We will use Jupyter Notebook as part of the Anaconda distribution, which can be downloaded from the official website (https://www.anaconda.com/).

Once installed and launched, we find ourselves in the home directory, which is the folder from which Jupyter Notebook was launched.

Press the New menu and select Python 3 to open a new notebook.

By clicking on the name of our laptop in a hat (now called Untitled), you can rename it. Let's rename the notebook to Lesson1.

At the top there is a toolbar that allows you to control our laptop. Here are some of the functions available through it.

In addition to intuitive items, the File menu offers several very important options.

The Edit menu contains actions on the cells. Here you can cut, copy, insert cells (both at the top and bottom of a given cell), delete. 

You can also separate cells or merge cells into one, and you can move cells up and down. In the same menu, there is a very useful function called Find and Replace, which allows you to search for and replace cells in your notebook by their contents.

Using the Insert menu, you can create new cells in your notebook, both above and below this menu. In the Cell menu, there are options associated with starting cells.

Using the Kernel menu, you can manage the processes taking place in our notebook. With the Interrupt option, you can interrupt the current process (the same can be done with a specific button on the

With Restart, you can fully reboot your laptop, and with Shutdown, you can simply stop it completely.
The toolbar also has a drop-down menu where you can select the type of cell. 

Here we will mainly use two options - Code and Markdown . Code is the default cell type. In these cells, you can type the programme code and run it. Markdown - a cell with text. Here you can type text using the Markdown syntax (https://ru.wikipedia.org/wiki/Markdown) and LaTeX (https://ru.wikipedia.org/wiki/LaTeX).

### Hot Keys

Jupyter Notebook also allows the use of hotkeys to simplify and speed up your work there. For example, here are a few ways to quickly start a current cell:

- Shift + Enter - start the cell and go to the next 
- Ctrl + Enter - start the cell and stay in it

A list of hotkeys can be found in the Help Keyboard Shortcuts menu.

When writing code in a cell, it is also useful to use the Tab key: it gives you a hint on which commands begin with these letters. For example, you can type in the cell pr and then press Tab and we will get a window with all the commands that start with pr .

If you want to know more details about what a function does, what arguments it accepts, etc., you will be given a hint. - here are a few ways to call up documentation for a function:

- Type the name of this function (e.g. print ) and press Shift + Tab
- Place a question mark before this function (e.g. ?print) and start this cell

You can also run commands from the command line of your operating system by placing a symbol ! in front of the command to be launched. For example, in the Windows operating system, the command !dir will display the contents of the folder in which you are located.

### Magic Commands

You can run so-called magic commands in Jupyter Notebook. The list of such commands can be viewed as follows: type %lsmagic in the cell and start the cell. Commands that start with one sign
%, apply to only one line of code, and those starting with two characters apply to the entire cell. 

Here are some magic commands:

- %run script.py - starts the code from files with the extension .py or from other laptops
- %load script.py - uploads the code from the file inside the cell, and the %load command itself becomes commented on
- %pycat script.py - downloads the code from the file to a pop-up window at the bottom of the page
- %% time - shows how long teams from this cell have been executed
- %%timeit - starts the content of a given cell several times and counts the average run time

## Contributing

Pull requests are welcome.

## Source

[Geekbrains](https://geekbrains.ru)
