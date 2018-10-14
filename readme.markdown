# Workshop: Text Analysis and Machine Learning at WU

The workshop is divided into five sections, each taking between 60 and 75 minutes, with breaks between sections.
As our time and progress allows, we will spend more time with the later topics and their associated materials.


## Schedule

topic | time
------|-----
Overview and Tools | 9:00-10:00
Python Basics | 10:15-11:15
Data Handling | 12:30-13:45
Text Analysis | 14:00-15:00
Machine Learning | 15:15-16:30


## Materials

There is a notebook and slide deck for each section.
Also, there is an `environment.yml` file for setting up your Anaconda environment, using the instructions below.


## Importing the Anaconda environment.

1. Open the Anaconda Navigator app.
1. On the left, click Environment.
1. At the bottom of the resulting main window, click Import.
1. In the resulting popup, click the folder icon, navigate to the `environment.yml` file, and click Open.
1. Back in the import popup, the environment name should be filled in automatically from the file, `workshop` in this case. Click Import.
1. Wait for the packages for the environment to be downloaded and installed. This could take a few minutes.

**Note:** there is also a file named `environment_full.yml`.
This file is much more specific about particular software versions, and it is largely specific to both macOS and particular hardware.
I include it for documentation reasons, but you should generally use the more general (i.e. compatible) `environment.yml`.

## Resolving Potential Setup Issues

In some testing, it seems that Anaconda is not reliably installing the `nytimesarticle` package used in section 03. To resolve this issue, do the following:

1. Open a terminal (on Windows, use the "Anaconda (64-bit)" prompt in the start menu).
1. Activate the `workshop` environment using the command `conda activate workshop`.
1. Install the package using the command `pip install nytimesarticle`. There may be warnings or errors that are not relevant for our purposes, so long as you see that `nytimesarticle` was installed successfully.


Similarly, some features of TextBlob (mainly used in section 04) depend on text corpora that may not have been automatically installed. To resolve this issue, do the following:

1. Open a terminal (on Windows, use the "Anaconda (64-bit)" prompt in the start menu).
1. Activate the `workshop` environment using the command `conda activate workshop`.
1. Install the corpora using the command `python -m textblob.download_corpora`. Again, there may be warnings or errors that are not relevant for our purposes, but you should see a series of successful downloads.


## About Jason

Jason T. Kiley is an assistant professor at Oklahoma State University.
His research examines the interplay of audience perceptions of firms, impression management, and their associations with outcomes, including recent publications in the Academy of Management Journal and Strategic Management Journal.
As part of his work, he works to advance the use of software to increase the range, efficiency, and rigor of conducting empirical research.
He is a co-organizer of the annual AOM Content Analysis PDW, and his published and in-progress work often uses state-of-the-art content analysis techniques, including recent work with semantic text analysis and machine learning.
