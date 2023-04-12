# Extorr RGA Python Interface

This project provides a Python interface for controlling and acquiring data from an Extorr Residual Gas Analyzer (RGA). The interface uses the Extorr software's built-in ActiveX automation server to communicate with the RGA.

---

# Project Description

This project aims to interface with an Extorr Residual Gas Analyzer (RGA) using Python. The Extorr RGA is a scientific instrument used for gas analysis, particularly in vacuum systems. It can detect and measure the partial pressures of various gas species at different mass-to-charge ratios. The objective of this project is to develop a software application that can interface with the Extorr RGA to control the scan parameters, acquire RGA data, and process the acquired data.

# File Descriptions

`extorr.py`
This file contains the ExtorrRGA class, which is the core class for interfacing with the Extorr RGA using Python. The class uses the Extorr software's ActiveX automation server to control the scan parameters, start the scan, check if the scan is complete, and get the acquired RGA data.

`main.py`
This file contains the main script that uses the ExtorrRGA class to interface with the Extorr RGA. It creates an instance of the ExtorrRGA class, sets the mass range for the scan, starts the scan, waits for the scan to complete, gets the acquired RGA data, and prints the mass-to-charge ratios and partial pressures of the detected gas species.

`data.py`
This file contains a function called process_data that can be used to process the acquired RGA data. The function takes the mass-to-charge ratios and partial pressures of the detected gas species as input and returns a processed version of the data, such as the total pressure.

`test_extorr.py`
This file contains unit tests for the ExtorrRGA class. The tests check the functionality of the set_mass_range, start_scan, and get_data methods of the class.

`test_data.py`
This file contains unit tests for the process_data function in the data module. The tests check that the function correctly calculates the total pressure from the partial pressures of the detected gas species.

---

## Installation
To install the project, first clone the repository to your local machine:

`git clone https://github.com/yourusername/extorr-rga-python-interface.git`

Then, create and activate a virtual environment for the project:

`virtualenv env`
`source env/bin/activate`

Install the project dependencies using pip:

`pip install -r requirements.txt`

---

## Usage
To run this program, you will need to install the required dependencies listed in the requirements.txt file by running the command pip install -r requirements.txt.

Once the dependencies are installed, you can run the program by running the main.py script in the terminal using the command python main.py.

To use the interface, simply import the ExtorrRGA class from the extorr.py module and create an instance of the class:

`from extorr import ExtorrRGA`
`rga = ExtorrRGA()`

You can then use the methods of the ExtorrRGA class to control the RGA and acquire data. For example, to set the mass range for the RGA to scan and start the RGA scan:

`rga.set_mass_range(1, 40)`
`rga.start_scan()`

To retrieve the acquired RGA data:
`data = rga.get_data()`

---

## Project Structure


The project has the following file structure:

```
.
├── README.md
├── requirements.txt
├── extorr.py
├── data.py
└── tests
    ├── test_extorr.py
    └── test_data.py
```

The extorr.py module contains the ExtorrRGA class for interfacing with the Extorr software's ActiveX automation server. The data.py module contains functions for processing and analyzing RGA data. The tests directory contains test files for each module.

---

## Contributing
Contributions to the project are welcome! If you find a bug or have an idea for a new feature, please submit an issue on the project's GitHub page. If you'd like to contribute code, please fork the repository and submit a pull request with your changes.


**Edit a file, create a new file, and clone from Bitbucket in under 2 minutes**

When you're done, you can delete the content in this README and update the file with details for others getting started with your repository.

*We recommend that you open this README in another tab as you perform the tasks below. You can [watch our video](https://youtu.be/0ocf7u76WSo) for a full demo of all the steps in this tutorial. Open the video in a new tab to avoid leaving Bitbucket.*

---

## Edit a file

You’ll start by editing this README file to learn how to edit a file in Bitbucket.

1. Click **Source** on the left side.
2. Click the README.md link from the list of files.
3. Click the **Edit** button.
4. Delete the following text: *Delete this line to make a change to the README from Bitbucket.*
5. After making your change, click **Commit** and then **Commit** again in the dialog. The commit page will open and you’ll see the change you just made.
6. Go back to the **Source** page.

---

## Create a file

Next, you’ll add a new file to this repository.

1. Click the **New file** button at the top of the **Source** page.
2. Give the file a filename of **contributors.txt**.
3. Enter your name in the empty file space.
4. Click **Commit** and then **Commit** again in the dialog.
5. Go back to the **Source** page.

Before you move on, go ahead and explore the repository. You've already seen the **Source** page, but check out the **Commits**, **Branches**, and **Settings** pages.

---

## Clone a repository

Use these steps to clone from SourceTree, our client for using the repository command-line free. Cloning allows you to work on your files locally. If you don't yet have SourceTree, [download and install first](https://www.sourcetreeapp.com/). If you prefer to clone from the command line, see [Clone a repository](https://confluence.atlassian.com/x/4whODQ).

1. You’ll see the clone button under the **Source** heading. Click that button.
2. Now click **Check out in SourceTree**. You may need to create a SourceTree account or log in.
3. When you see the **Clone New** dialog in SourceTree, update the destination path and name if you’d like to and then click **Clone**.
4. Open the directory you just created to see your repository’s files.

Now that you're more familiar with your Bitbucket repository, go ahead and add a new file locally. You can [push your change back to Bitbucket with SourceTree](https://confluence.atlassian.com/x/iqyBMg), or you can [add, commit,](https://confluence.atlassian.com/x/8QhODQ) and [push from the command line](https://confluence.atlassian.com/x/NQ0zDQ).

---

## License
This project is licensed under the MIT License. See the LICENSE file for details.