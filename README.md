# Data Modeling with Apache Cassandra

## Intro

A startup called _Sparkify_ wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analytics team is particularly interested in understanding what songs users are listening to. Currently, they don't have an easy way to query their data to generate results, which resides in a directory of JSON logs on user activity on the app, as well since the data reside in a directory of CSV files on user activity on the app.

They'd like a data engineer to create an Apache Cassandra database which can create queries on song play data to answer the questions. This project creates a database for analysis along with testing the database by running queries given by the analytics team.

## Project Description

In this project, I apply data modeling with Apache Cassandra and build an ETL pipeline using Python. Data is modeled by creating tables in Apache Cassandra to run the queries.

## Getting Started

My operating system is a Mac so the installation instructions reflect this system. The code editor used was Atom. Most of the files and configurations were provided by Udacity.

### Installing Git

Git is already installed on MacOS, but these instructions are to ensure we have the latest version:

1. go to [https://git-scm.com/downloads](https://git-scm.com/downloads)
2. download the software for Mac
3. install Git choosing all the default options

Once everything is installed, you should be able to run `git` on the command line. If usage information is displayed, we're good to go!

### Configuring Mac's Terminal (OPTIONAL)

Git can be used without reconfiguring the terminal but doing so makes it easier to use.

To configure the terminal, perform the following:

1. download [udacity-terminal-config.zip](http://video.udacity-data.com.s3.amazonaws.com/topher/2017/March/58d31ce3_ud123-udacity-terminal-config/ud123-udacity-terminal-config.zip)
2. Move the `udacity-terminal-config` directory to the directory of your choice and name it `.udacity-terminal-config`(Note the dot in front)
3. Move the `bash-profile` to the same directory as in `step 2` and name it `.bash_profile`(Note the dot in front)
    * If you already have a `.bash_profile` file in your directory, transfer the content from the downloaded `bash_profile` to the existing `.bash_profile`

**Note:** It's considerably easier to just use
`mv bash_profile .bash_profile`
and `mv udacity-terminal-config .udacity-terminal-config`
when moving and renaming these files in order to avoid mac system errors

### First Time Git Configuration
Run each of the following lines on the command line to make sure everything is set up.
```
# sets up Git with your name
git config --global user.name "<Your-Full-Name>"

# sets up Git with your email
git config --global user.email "<your-email-address>"

# makes sure that Git output is colored
git config --global color.ui auto

# displays the original state in a conflict
git config --global merge.conflictstyle diff3

git config --list
```

### Git & Code Editor

The last step of configuration is to get Git working with your code editor. Below is the configuration for Atom. If you use a different editor, then do a quick search on Google for "associate X text editor with Git" (replace the X with the name of your code editor).
```
git config --global core.editor "atom --wait"
```

### Install Cassandra on MacOS

This [link](https://gist.github.com/hkhamm/a9a2b45dd749e5d3b3ae) offers useful steps to installing Cassandra on Mac.

### Install Cassandra wrapper

**This project uses a python wrapper/ python driver called cassandra to run the Apache Cassandra queries. This library should be preinstalled but in the future to install this library you can run this command in a notebook to install locally:**
`! pip install cassandra-driver`

### requirements.txt

Refer to [requirements.txt](https://github.com/rtelles64/data_modeling/blob/master/requirements.txt) for project/environment packages.

## Datasets

There is one dataset being worked with: `event_data`. The directory of CSV files partitioned by date. Here is an example of filepaths to two files in the dataset:
```
event_data/2018-11-08-events.csv
event_data/2018-11-09-events.csv
```

## Version

This project uses `Python 3`

## Author(s)

* **Roy Telles, Jr.** *(with the help of the Udacity team)*

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* I would like to acknowledge and give big thanks to Udacity and team for this excellent resume-building experience
