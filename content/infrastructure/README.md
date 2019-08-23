# Software

---

| <CENTER>OS</CENTER>    | | <CENTER>Status</CENTER> |
| ------- | ----- | -----------------|
| Linux & macOS  | | [![Build Status]() |
| Windows |  | [![Build status]() |

---

This course is best followed if you can reproduce the examples and tutorials provided with it. To do so, you will need to install in your machine a series of software packages. These are all open-source and available for free to download.

## Complementary material to this guide

This guide assumes you have the following additional files, available to download by clicking (to download them, right click on the link and select the "save as" option):

* [`install_stats_stack.yml`](content/infrastructure/install_stats_stack.yml)
* [`check_stats_stack.ipynb`](content/infrastructure/check_stats_stack.ipynb)

## Installation

### Conda

The easiest way to install locally and natively the software stack required is to install a full scientific Python distribution. Although other good alternatives are also available (e.g. [Canopy](https://www.enthought.com/products/canopy/), [Sage](http://www.sagemath.org)), we recommend to install [Miniconda](https://conda.io/miniconda.html). Make sure, whichever option you pick, to install a **Python 3.6** version, NOT Python 2. Please follow the instructions provided in the link for installation.

Once you have a fully working conda installation in your computer, you can setup an isolated environment that contains all the required libraries by running the install script provided with this guide. Exact instructions vary depending on the platform you are on. 

Open up a terminal ("Anaconda Command Prompt" in Windows, "Applications --> Utilities --> Terminal" in macOS and  "ctr+alt+T" in Linux) and run the following commands:

* Navigate to the folder where this file is (e.g. Downloads):

    ```
    cd /path/to/folder/
    ```

* Execute the following command:

    ```
    conda-env create -f install_stats_stack.yml
    ```

* Once this has run, you should be able to activate the environment:

    ```
    conda activate stats
    ```

## Check

To check things have installed correctly, an additional file is included, `check_stats_stack.ipynb`. To run the check, open a terminal (macOS/Linux) or the Anaconda Command Prompt (Windows), navigate to the folder as showed above and activate the environment:

    ```
    conda activate stats
    ```

You should now see `(stats)` on the beginning of the line at the terminal/command prompt. You can now run the test as:

`jupyter nbconvert --execute check_stats_stack.ipynb`

This will run and, when finished, produce an HTML file in the same folder. Open it and check there are no errors reported. If that is the case, you are good to go!


