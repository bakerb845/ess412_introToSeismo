# Introduction to Seismology Jupyter Notebooks

These are the Jupyter notebooks for the UW ESS 412/512 winter quarter introduction to seismology class.

These are intended to be run with Python 3.x where x can be 4 or 5.  These should also be accessible via [Microsoft Azure](https://notebooks.azure.com).

## Prerequisites

These are Python3.5 notebooks.  They will subsequently require

1. Python version 3.5.  Version 3.6 may also work.  The 2.x series is being deprecated so I'm trying to avoid it.
2. [ObsPy](https://github.com/obspy/obspy/wiki).
3. [Jupyter] notebooks.
4. [Git](https://git-scm.com/).
5. [basemap](https://matplotlib.org/basemap/)

Optional - I strongly recommend installing Python with [Anaconda](https://conda.io/docs/user-guide/install/index.html).  In this instance you'll end up with Python3.6 and have to add

    conda config --add channels conda-forge

Alternatively, you can use these notebooks in a cloud environment via [Microsoft Azure](https://notebooks.azure.com).  However, this will require that you register with Microsoft.

## Staying Up-To-Date

This repository will be populated as the class unfolds.

### If working at a terminal

To stay up to date change your working directory to where the git repository is downloaded, e.g.,

    cd /path/to/ess412_introToSeismo

Then type

    git pull

This should pull the latest notebooks and you'll up-to-date.  

### If working on Azure

To stay up to date on Azure open a "Terminal."  Then type

    git pull

This should pull the latest notebooks and you'll be up-to-date. 

### Git is sassing you

You probably modified a file without changing the name/copying it to your local directory.  In git's complaints will likely be offending file names.  Let's say nisqually.ipynb is causing issues.  You can do a few things here.

(1)  Change the offending file names

    mv niqually.ipynb to nisqually_myName.ipynb

(2)  Commit your change.  This may ultimately lead to a merge conflict but git can be pretty clever so give it a try.

    git add nisqually.ipynb
    git commit -m "I've modified this file while doing my homework.  Maybe I'll follow the directions next time."

## Usage

Here are some ideas on usage for those working at a terminal and those working on Azure.

### If working at a terminal

In this option locate the notebook in the git repo structure.  Change directories to where you are doing your work, e.g.,

    cd /path/to/my/seismology/homework

Now copy it to your working directory, e.g., 

    cp /path/to/ess412_introToSeismo/directory/notebook.ipynb ./notebook_myName.ipynb

Renaming the file will prevent git from destroying your file during a git pull phase. 

Then run the notebook

    /path/to/anaconda3/bin/jupyter notebook

In a web-browser you will see notebook\_myName.ipynb.  Select it and click "Run".

### If working on Azure

In this option locate the appropriate notebook in the library structure.  For example, let's call it notebook/notebook.ipynb.  Then rename notebook.ipynb by right-clicking and entering notebook\_myName.ipynb.  This will prevent git from destroying your work during a git pull phase.

Now select the renamed notebook and type "Run".

## Directories

This is an overview directories and files contained within are described.

1. introToSeismology.ipynb - A quick introductory script to basic Python.
2. nisqually.ipynb - This is the Nisqually 2001 event recorded at station KEV.  It is an introduction to waveform interpretation and major seismic signals that we'll discuss in the class. 

