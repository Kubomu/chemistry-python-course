# Python for Applied Chemistry

[![Launch in Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Kubomu/chemistry-python-course/main?urlpath=lab)
[![Python 3.9+](https://img.shields.io/badge/python-3.9%2B-blue.svg)](https://www.python.org/downloads/)

A short, hands-on course that teaches Python by using it to do real chemistry: analysing lab data, plotting results, and exploring reactions. Every lesson is a Jupyter notebook you can run in your browser without installing anything.

New here? Go straight to [Run it in your browser](#run-it-in-your-browser). You will be running real chemistry code in a minute or two.

## Table of Contents

- [Run it in your browser](#run-it-in-your-browser)
- [What you will learn](#what-you-will-learn)
- [The lessons](#the-lessons)
- [Datasets](#datasets)
- [Run it on your own machine](#run-it-on-your-own-machine)
- [A note for Google Colab users](#a-note-for-google-colab-users)

## Run it in your browser

The easiest way to start is Binder. Click the button below. Binder reads this course's `requirements.txt`, installs everything for you, and opens Jupyter in your browser. Nothing to download.

[![Launch in Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Kubomu/chemistry-python-course/main?urlpath=lab)

The first launch takes a minute or two while Binder sets up the environment. After that, open a lesson from the file list on the left and run each cell with Shift and Enter.

Prefer to open one specific lesson directly? Use the per-lesson buttons in [The lessons](#the-lessons) below. Each lesson has a Binder button (everything preinstalled) and a Colab button (fast to open, see the [Colab note](#a-note-for-google-colab-users)).

## What you will learn

- Reading and cleaning real lab data with pandas
- Doing calculations with numpy
- Turning numbers into clear plots with matplotlib
- Working with reactions and chemical quantities using chempy
- Building the habit of exploring data in a notebook, one cell at a time

No prior Python is assumed. Basic chemistry (concentrations, reactions, titrations) is helpful but each idea is explained as it comes up.

## The lessons

Work through them in order. Each button opens that lesson ready to run.

| Lesson | Topic | Open (everything ready) | Open (fast) |
|--------|-------|-------------------------|-------------|
| 1. Python Basics for Chemistry | Variables, lists, and simple calculations, using chemistry examples | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Kubomu/chemistry-python-course/main?labpath=Lesson1_Python_Basics_for_Chemistry.ipynb) | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Kubomu/chemistry-python-course/blob/main/Lesson1_Python_Basics_for_Chemistry.ipynb) |
| 2. Data Analysis and Plotting | Loading CSV lab data with pandas and plotting it with matplotlib | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Kubomu/chemistry-python-course/main?labpath=Lesson2_Data_Analysis_Plotting.ipynb) | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Kubomu/chemistry-python-course/blob/main/Lesson2_Data_Analysis_Plotting.ipynb) |
| 3. Cheminformatics with ChemPy | Balancing reactions and working with chemical quantities | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Kubomu/chemistry-python-course/main?labpath=Lesson3_Cheminformatics_ChemPy.ipynb) | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Kubomu/chemistry-python-course/blob/main/Lesson3_Cheminformatics_ChemPy.ipynb) |

There are also slides, `Python_for_Applied_Chemistry.pptx`, that introduce the course.

## Datasets

The lessons use small, real CSV datasets kept in the `datasets/` folder:

- `nwsc_water_quality.csv` - water quality measurements
- `reaction_kinetics.csv` - reaction rate data over time
- `titration_data.csv` - titration readings

When you launch with Binder or Codespaces these come along automatically. In Colab they load straight from this repository.

## Run it on your own machine

If you would rather not use the browser:

1. Clone the repository:
   ```bash
   git clone https://github.com/Kubomu/chemistry-python-course.git
   cd chemistry-python-course
   ```
2. Install the packages:
   ```bash
   pip install -r requirements.txt
   ```
3. Start Jupyter and open a lesson:
   ```bash
   jupyter lab
   ```

You can also open the folder in GitHub Codespaces (Code button, then Codespaces) and the environment installs itself.

## A note for Google Colab users

Colab opens instantly and already has pandas, numpy, and matplotlib, so Lessons 1 and 2 run as is. Lesson 3 uses chempy, which Colab does not include by default. When you open Lesson 3 in Colab, add a new cell at the very top and run this once:

```python
!pip install chempy
```

Then run the rest of the notebook normally. Binder does not need this step because it installs everything from `requirements.txt` for you.
