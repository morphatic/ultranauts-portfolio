# Morgan's SQL Code Sample (with Python and Jupyter Notebook)

[<abbr title="Structured Query Language">SQL</abbr>](https://en.wikipedia.org/wiki/SQL) is the nearly universal language of relational databases. As such, it is a VERY valuable skill for Ultranauts engineers, whether on <abbr title="Software Test Automation">STA</abbr> or <abbr title="Data Quality Engineering">DQE</abbr> projects. This project demonstrates my ability to:

1. Frame relevant business questions in human-readable English
2. Convert those English questions into runnable SQL queries
3. Draw reasonable conclusions from the output of those queries

<!-- omit in toc -->
## <abbr id="toc" title="Table of Contents">TOC</abbr>

* [Timeframe](#timeframe)
* [Background](#background)
* [What To Look At](#what-to-look-at)
* [Launch the Jupyter Notebook to Run the Code](#launch-the-jupyter-notebook-to-run-the-code)
* [Thoughts and Comments](#thoughts-and-comments)
* [Screenshots](#screenshots)
* [Questions](#questions)

## Timeframe

This code was written in November 2022.

## Background

This project represents the application of the skills I learned while following the [Data Profiling Learning Path](https://docs.google.com/document/d/1tBGKNR040FbKgm8ZToJY-2XDIOyfdWplTI30vuTZoGg/edit?usp=sharing) established by the Ultranauts <abbr title="Learning & Development">L&D</abbr> team. It demonstrates not only that I completed the learning path, but understand and can apply the things I learned in it. Furthermore, it is an example of the practical combination of my Python skills, and documentations skills, since I used a [Jupyter Notebook](https://jupyter.org) to organize and document my samples.

The sample database I used in this project is the [Chinook database](https://github.com/lerocha/chinook-database) implemented with [SQLite](https://www.sqlite.org/index.html). I did not create this database. It is a free, open-source resource that anyone can use while learning, or in my case, demonstrating what they have learned with SQL. That said, the questions posed in the Jupyter Notebook, and more importantly the SQL written to get the answers from the database, were entirely written by me. Here is the Chinook data model, for reference, which shows that it is a "typical" DB structure one might encounter for a small business.

![Chinook Database Entity Relationship Diagram](chinook-er-diagram.png)

## What To Look At

This project primarily demonstrates my capability to write SQL queries. It also shows these capabilities:

* Creating and managing a project on GitHub
* Setting up a Python project meant for collaboration and distribution
* Clear, useful documentation
* Use of off-the-shelf tools like Jupyter Notebooks

## Launch the Jupyter Notebook to Run the Code

0. You must have `git` and `python` (v3.3 or later) installed on your computer
1. From a terminal, clone this repo
2. Navigate to the `sql/` folder

      <!-- language: lang-sh -->
        cd ultranauts-portfolio/sql
3. Instantiate and activate Python virtual environment in this directory with (note OS-specific instruction):

      <!-- language: lang-sh -->
        python -m venv venv
        source ./venv/bin/activate # activate command on Mac
        source ./venv/Scripts/activate # activate command on Mac
4. Install the required packages (these will NOT install globally, just in the virtual environment):

      <!-- language: lang-sh -->
        pip install -r requirements.txt
5. Once requirements are installed you can launch the Jupyter notebook with:

      <!-- language: lang-sh -->
        jupyter notebook
6. Open the Jupyter Notebook in your web browser. The code examples are documented there, and can be run from within the browser.

## Thoughts and Comments

Here are some of the things I learned while doing this project.

* Many tutorials suggest that beginners install [Anaconda](https://www.anaconda.com/) when setting up their systems to use Jupyter Notebooks. **I THINK THIS IS A VERY BAD IDEA!!!** Anaconda is HUGE, has the tendency to "take over" your system and be VERY difficult to remove. It can automatically change global Python settings that make it difficult or impossible to work with previously-existing Python projects on your computer. This is especially frustrating if you are a beginner.
* Thing 2
* Thing 3...

## Screenshots

My opportunities to apply my SQL knowledge on actual Ultranauts projects have been limited. Here is a screenshot of some SQL I contributed to a recent project as evidence that I am applying these skills in practice. That said, I didn't feel this one sample was sufficient to capture the full extent of my ability with this capability.

![some screenshot](screenshot1.png)

## Questions

If you have any questions about these code samples or about SQL, Python, and/or Jupyter Notebooks, please reach out to me on Slack, or by email at <a href="mailto:mbenton@ultranauts.co">mbenton@ultranauts.co</a>.
