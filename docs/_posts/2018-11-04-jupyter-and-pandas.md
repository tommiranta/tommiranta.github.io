---
layout: post
title:  "Jupyter + Pandas = Excel on steroids"
date:   2018-12-02
categories: python
---
![Jupyter](/assets/images/2018-11-04-jupyter-and-pandas/jupyter1.png)

Exploratory data analysis and cleaning data is one of the most important
aspects of any machine learning task. One cannot get the best results out of a
model without properly understanding the data that your work with. Thus I
decided to start my learn machine learning journey by getting to know Pandas
and Jupyter. Little did I know what an impact it would have on my daily work,
even if not working directly with data science tasks. In this article I will
introduce you to Pandas and Jupyter and how to get started using them. I will
tell about its benefits and how it has partially replaced the work with Excel
and improved my efficiency. It's not the best fit for all of your  tasks so I
will also bring up scenarios where you're probably better off using other tools.

## About Jupyter and Pandas

[Jupyter](http://jupyter.org/) is an interactive web application that allows
you to run and visualize live code (Python in my case) instead of running it as
an script or application. It also supports adding narrative text, which you to
create reports within the tool itself. [Pandas](https://pandas.pydata.org/) is
an easy-to-use data structures and data analysis library. Combined these tools
provide possibilities for data cleaning and transformation, data analysis, data
visualization, and simple statistical modeling. The true power of Jupyter
unfolds because you have the possibility to utilize all the libraries available
for Python. [Seaborn](https://seaborn.pydata.org/) for statistical
visualization, [scikit-learn](http://scikit-learn.org/stable/) for machine
learning, [keras](https://keras.io/) for deep learning to name a few.

![Jupyter](/assets/images/2018-11-04-jupyter-and-pandas/jupyter2.png)

## Benefits & Drawbacks

I have used Jupyter + Pandas in many occasions, such as; analysis of hourly
data for budgetary follow-up and invoicing, helping locate inactive mobile
subscriptions, clean-up of various data before passing it onward as an Excel
workbook, analysis of survey results, and analysis of bug tracker data. Here
are some of the benefits I've come across:

- *Python ecosystem* - Since Python is a programming language you have almost
endless possibilities with what you can do with data. Re-use of code, utilize
3rd party libraries, automate work recurring tasks after analysis in Jupyter etc.
- *Importing data from more unconventional formats* - Although Excel provides
basic possibilities for importing tables from web pages it does not come near
to the possibilities provided by [web scraping](https://en.wikipedia.org/wiki/Web_scraping)
libraries or importing a table directly from a [PDF document](https://github.com/socialcopsdev/camelot).
- *Efficient filtering, combining and aggregation of data* - Pandas allows you
to do database-like actions such as joining, grouping and querying. In
addition, it has pivot functionality similarly to Excel.
- *Quick prototyping and visualization* - Unless I work with simple data I
often reach the desired results quicker  using Pandas than with Excel. This
although I consider myself a quite seasoned user of Excel.

While there are lots of benefits, there are also occasions when this might not
be the best option for you. The main reason being a steep learning curve unless
you have some kind of background in programming. I wouldn't recommend anyone to
learn Python and Pandas for the sake of replacing Excel. Use Excel if you're
working with simple data. While the Python ecosystem allows for great
customization regarding graphs and other visual components you're probably
better off sticking to Excel if the wanted type of visualization and
customization is available.

## How to get started

There are several ways to install Python & Pandas on your computer. Probably
the quickest way to get up and running if you're starting from scratch is to
install the [Anaconda Distribution](https://www.anaconda.com/download/), which
provides everything you need with one installer. You can install the libraries
using pip in case you already have the Python environment installed on your
computer. Open a command prompt/terminal and execute:

```shell
pip install pandas jupyter xlrd openpyxl
```

`xlrd` and `openpyxl` libraries are required in order to read and write Excel
workbooks from Pandas.

Installation instructions:
[Anaconda](https://docs.anaconda.com/anaconda/install/),
[Python](https://realpython.com/installing-python/),
[Pandas](https://pandas.pydata.org/pandas-docs/stable/install.html),
[Jupyter](http://jupyter.org/install.html).

You can start Jupyter once you have installed the needed packages by
double-clicking the *Jupyter Notebook* icon installed by Anaconda or by
executing the following command:

```shell
jupyter notebook
```

Starting Jupyter should automatically open up the application in your default
web browser. In case this doesn't happen try navigating to
`http://localhost:8888`, which is the default address when running Jupyter on
your own computer.   The next step is to get acquainted with Jupyter and
Pandas. The internet is full of good resources, here are some to get you
started:

- [Jupyter Notebook Tutorial: The Definitive Guide](https://www.datacamp.com/community/tutorials/tutorial-jupyter-notebook)
by Datacamp
- [Jupyter Notebook for Beginners: A Tutorial](https://www.dataquest.io/blog/jupyter-notebook-tutorial/)
by Dataquest
- [10 Minutes to pandas](https://pandas.pydata.org/pandas-docs/stable/10min.html)
, by Pandas
- [Cookbook](https://pandas.pydata.org/pandas-docs/stable/cookbook.html#cookbook)
, by Pandas
- [Data Analysis with Python and Pandas](https://pythonprogramming.net/data-analysis-python-pandas-tutorial-introduction/)
video tutorial by Pythonprogramming
- [Data Analysis with Pandas and Python](https://www.udemy.com/data-analysis-with-pandas)
on Udemy by Boris Pashkaver

Personally I have experience from the course on Udemy, which provided an
comprehensive overview of what you can do with Pandas. Especially in the
beginning, I often relied on the notebooks created during the course when
working on real world problems. Hope this has gotten you excited to give Pandas
a try and let me know how you utilize Pandas and/or Jupyter in your work!
