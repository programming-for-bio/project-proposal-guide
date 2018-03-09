
# Project Guide and Instructions

Course projects are meant to provide an exercise in which you explore
and learn to use new coding tools on your own that we have not yet covered
in class. The exact format is flexible and the finished product could encompass
a number of different things. Below I list the rules, restrictions, and 
recommendations for project proposals as well as several example ideas.

## Format/Deadlines
**Proposal:** one page essay and create project GitHub repo -- *due 3/21*.   
**Presentation:** presentation of proposal and progress so far (10 minutes with 
questions) -- *4/23 and 4/30.*    
**Final project:** GitHub repo with code, data, example notebooks, and final
one page essay -- *due 5/11*.  


## Grades: 
As stated in the course syllabus, the project proposal, presentation and 
final form make up a significant portion of your total course grade: 
+ **Proposal:** 5%  
+ **Presentation:** 5%  
+ **Final project:** 15%  


## Pre-proposal email:
Even if we have already spoken about your project idea you should send me an 
email with the subject line `PDSB project` and a very short and rough 
description of your idea before writing your proposal (de2356@columbia.edu). 
I will respond quickly with advice as to whether it sounds feasible. 
Before you send it, however, please read the instructions below carefully. 
Choosing a topic is one of the most important parts of your project, and you
should think deeply about it before making your decision. You have almost two 
weeks before the proposal is due, which is plenty of time to look for 
appropriate data sets and investigate potential tools for analyzing them. 
Your project may change between the proposal and final submission.

## Proposal Essay Instructions:
Proposals should be approximately one page single-spaced (including references) 
answering the following five questions.  

1. **The problem**: What is the problem you wish to solve?
2. **The data**: What is the data you will analyze and where is it from?
3. **The tools**: What computational tools will you use to solve the task?
4. **The novelty**: Why is this novel?
5. **The goal**: What is your envisioned product at the due date and after?


## Proposal Details:
1. **The problem:** Choose a problem that is of interest to you and is
appropriately difficult given the timescale of the project (~7 weeks).
This could be to write a program or library that can accomplish 
some repetitive task, or to learn to use an existing library for statistically 
analyzing a particular type of data (though this must be sufficiently complex or
combined with further programming), or to develop a tool for visually representing
data or results that is novel. See the *ideas* section at the end of this file. 

2. **The data:** Part of this exercise is to find appropriate data to answer the
question you are interested in. This could be data that you have collected
as a graduate student. It could be data that is available from a professor 
that you know. It could be data that you generate yourself. 
Or, for most people, it will likely be data that you find in
an online database, e.g., from a published study. 

3. **The tools:** Why did you choose to use these tools? What other software
tools are likely to be used in your project? Is your method a 
reimplementation of an existing method, is it a pipeline? 

4. **The novelty:** In what way does your *problem + data + tools = novel*?
If you are not developing a new tool then your implementation should be 
novel (e.g., no one has previously applied this type of method to this data
set), and sufficiently difficult to implement.

5. **The goal:** Describe your envisioned final product, how can people use it?
You can list a short-term and theoretical long-term goal, for example, by 
the due date I plan to have a minimal working example that can accomplish x, 
with more time and effort my tool/method/example could also do y and z. 


### Restrictions on the above requirements: 

1. **The problem:** You must choose something feasible to accomplish in 
~7 weeks, and not too simple that it can be accomplished in a few days. This
may be hard to predict, but if you finish a project very quickly you will be 
expected to expand it beyond your initial proposal idea. If it turns out to be
much more difficult than you anticipated then you may scale back the idea to 
something more maneagable later. 

2. **The data:** You cannot use the example data set from the tutorial for a
software package. You should find data that has not yet been applied in the chosen 
software on a publicly available example. 
3. **The tools:** You must *write code* for your project. You should not be using
a click and point (GUI) based software like the argGIS GUI. However, your project
could propose developing something that is interactive and GUI based for users.
4. **The novelty:** Your project must include at least some 
tools/packages/languages we have not covered in class before spring break. 
5. **The goal:** You must propose to produce some kind of functional product 
by the due date. 
6. **other restrictions:** Your project must be individual, not a group effort, 
though we will have collaborative exercises to provide input on each others projects. 
7. **other restrictions:** Your project must follow guidelines of open and 
reproducible code we have followed so far in class: softare is freely available
and simple to install.

### GitHub repository structure: 

Create a new repository for your project and name it whatever you like 
(you can change the name later if you want as well). When you create the repo 
on GitHub select to create a README file and also add a LICENSE file and
select GPLv3 as the license type. 
Clone your repository and add the following four directories to it, which 
will make up the structure of your project. 
Your proposal and final essays can be markdown README files or docx files, 
whichever you prefer, and should be uploaded to the `documents/` 
directory by their due dates. See instructions below for the contents of the 
other directories.

```
PDSB-project/
    + notebooks/
    + data/
    + project/
    + documents/
    + README.md
    + LICENSE
```

+ `notebooks/`: This directory must contain at least one jupyter notebook 
that demonstrates your code on your test data set as an example implementation. 
This notebook should be nicely formatted and provide a formal tutorial that 
anyone else in class could run to reproduce your results and understand. 

+ `data/`: This directory should contain your data file unless your data are
downloaded directly from the internet. 

+ `project/`: The name of this directory can be whatever you want, it is the place
where you will store your code. 

+ `documents/`: This directory is where you will upload your proposal and 
final project essays.  

+ `README.md`: This README file should include (1) the name of your project, 
(2) a short description of what it does, (3) installation instructions, 
and (4) instructions to find examples in your notebooks directory. 


### Does my project have to be a Python program?
Your final project can be written in any programming language that you like. 
However, this is meant to be an exercise in creating something, not just in 
performing a statistical analysis, so you cannot simply load a CSV file into
R and run a predefined function on it using existing libraries. You should be
writing functions and creating a library/package, as we have learned to do 
in Python, or a command line tool. Writing R functions that extend the 
functionality of an existing library, such as by automating many calls to a 
function in it and parallelizing them, and/or better summarizing its results, 
and learning to package this together into an importable library would be a 
comparable exercise, since this is what is expected in Python. 
Regardless of which language you use, the code and 
dependencies must be easily installable by your classmates into a local software 
location like miniconda. (This is not overly difficult, but will require 
learning some installation methods similar to what we've learned so far for 
Python packages). 

## Some tools we have yet not covered in class

The following Python packages are interesting and powerful new libraries
that we have not had time to explore in class yet. They would be good topics
for project proposals. You may combine multiple tools for your project, 
since some of them, like a plotting tool, may be quite simple to learn, 
and so insufficient on its own as a project topic. 

To find more ideas search the web, there are many other libraries and tutorials 
out there, and don't limit yourself to just the official tutorials, most 
libraries will have many additional examples created by users that 
you can find on blogs, youtube videos, and publications. 


### Video and image analysis tools
+ [OpenCV](http://opencv-python-tutroals.readthedocs.io/en/latest/py_tutorials/py_tutorials.html)
+ [More docs for OpenCV](https://docs.opencv.org/3.4.1/d6/d00/tutorial_py_root.html)
+ [Scikit learn](http://scikit-learn.org/stable/tutorial/basic/tutorial.html)  

#### Statistical analysis tools
+ [PyMC3 Bayesian statistical modeling](http://docs.pymc.io/notebooks/getting_started.html)
+ [abcpmc Approximate Bayesian Computation](http://abcpmc.readthedocs.io/en/latest/installation.html)
+ [Statsmodels](http://www.statsmodels.org/stable/index.html)


#### AI/Machine learning tools
+ [Scikit learn](http://scikit-learn.org/stable/tutorial/basic/tutorial.html)  
+ [Tensorflow](https://www.tensorflow.org/tutorials/)  


#### Interactive visualization tools
+ [Dash visualization app](https://dash.plot.ly/gallery)
+ [Bokeh plots](https://bokeh.pydata.org/en/latest/)


#### Spatial analysis tools
+ [Overview of spatial methods](https://automating-gis-processes.github.io/2016/Lesson5-interactive-map-bokeh.html)
+ [Geopandas](http://geopandas.org/mapping.html)
+ [Google Earth Engine Python API](https://github.com/earthlab/tutorials/blob/master/documentation/intro-google-earth-engine-python-api.md)
+ [Cartopy](http://scitools.org.uk/cartopy/docs/latest/index.html)
+ [Folium](https://github.com/python-visualization/folium)


#### Biological or genomic data
+ [fwdpy](https://molpopgen.github.io/fwdpy11/) (forward in time demographic simulations)
+ [msprime](https://msprime.readthedocs.io/en/stable/) (coalescent demographic simulations)
+ [scikit-allel](https://scikit-allel.readthedocs.io/en/latest/)
+ [biopython](http://biopython.org/) (e.g., NCBI taxonomy data mining)


#### Web scraping tools
+ [Scrapy](https://scrapy.org/)
+ [requests](http://docs.python-requests.org/en/master/user/quickstart/)
+ [selenium](http://selenium-python.readthedocs.io/)



### Examples: 

The examples below are meant to represent the thought process that should go 
into choosing a project idea. Your grade will not necessarily reflect the 
complexity of your proposed project, but will reflect the effort that I infer 
(and will be able to see from your code and commits) that has gone into it. 
As stated before, you should choose a project idea that feels like it would 
be feasible within the >7 week time window. That should be plenty of time 
for you to expect that you can learn one or more new Python libraries well.

**Data sets**: Search here for large available databases: [https://catalog.data.gov/dataset](https://catalog.data.gov/dataset)


**Example 1 (complex -- combine multiple new tools, mines data, and write a package)**:  
You look through some examples from the tools above and think about 
biological questions that interest you. Let's say you are interested in bumblebee
diversity and conservation. You find a database with data on bee occurrences 
from museum collections that is accessible online through `https://bison.usgs.gov` 
(we'll learn more about this database in class soon, actually). 
From here you can download occurrence records with GPS points and collection 
years. There are >250K records for the genus *Bombus*. Using these data you propose
to examine how diversity or abundance of bees sampled in each state has changed 
over time. You propose to use the Python library `requests` to download 
occurence data. Then you will use `pandas` to organize the results, and perhaps
to filter the data before analyzing it. Next you will use `geopandas` and 
`folium` to plot how species diversity changed through time similar to one of 
the [example plots for geopandas](http://nbviewer.jupyter.org/github/python-visualization/folium/tree/master/examples/). Finally, if you have time you'll use PyMC3 to perform a Bayesian analysis 
similar to the [example in its Case-Study 2 tutorial](http://docs.pymc.io/notebooks/getting_started.html#Case-study-2:-Coal-mining-disasters) to identify whether 
there is a specific decade when bee diversity shifted dramatically. Your code
will be organized into a Python library so that in the end any user can enter
the name of a different genus and the program can reproduce the same type of 
analysis for that organism. 


**Example 2 (intermediate -- learn one new complex tool and write a package)**:  
You have behavioral data in the form of videos tracking the movement of some kind
of animals over time. You want to see if you can use a machine learning algorithm
to recognize a feature of the videos, such as an animal's face. You read the 
scikit learn tutorial and openCV tutorial and find [this video](https://www.youtube.com/watch?v=88HdqNDQsEk&t=315s) as a nice introduction. Based on your reading you 
decide to use OpenCV since you have video data. 
You find an image database of pictures of your type of animal that you use to 
train your algorithm, or you find one already available on google, such as a 
human facial recognition model, as described in the opencv tutorials. As a final 
product you will create a notebook to completely reproduce your analyses including
(1) loading all software; (2) downloading all required images or videos from 
an online source; (3) running your code (which will be written as
a user friendly Class object and library that can be imported); (4) 
and perform a statistical analysis comparing the results for several different
videos, which could be presented as a pandas dataframe of results 
or with plots. 


**Example 3 (simple -- learn one new complex tool, find a data set, and write a tutorial)**:   
You like visualization tools and want to develop a web-based app that users
can interact with and which shows some kind of rich data analysis and map 
side by side. You like the examples from the dash apps tutorial such as the 
[uber example](https://dash-uber-rides.plot.ly/). You will
find a similar dataset for something in New York so that you can reuse much of the 
code that is available for this example. Your final product will be a visualization
app that can be run locally on your computer and which could also be deployed 
to a website. If you have enough time you will try to figure out how to host 
it online. Your example notebook will act as a detailed tutorial about how you 
created your app so that other users can learn from your example. 




