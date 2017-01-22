# Setup

This page contains brief instructions on how to install the core applications that we will use in this course. During the course, these tools will be introduced slowly, and you will not be expected to become proficient in all or even most of these tools.

You can install them all at once, or gradually over the course. Feel free to play around with any of these tools

1. [Python Interpreter](#1-python-interpreter)
2. [GitHub Repository Manager](2-github-repository-manager)
3. [Atom Text Editor](#3-atom-text-editor)
4. [Slack Team Messenger](#4-slack-team-messenger)
5. [Tableau Visualization Platform](#5-tableau-visualization-platform)
6. [Google OpenRefine Data Scrubber](#6-google-openrefine-data-scrubber)
7. [Trifacta Data Wrangler](#7-trifacta-data-wrangler)

---

**!!! NOTE NOTE NOTE !!!**

Some of the following passages refer to your 'Terminal', to access it, follow the directions for your operating system...

**OSX:**

Go to your Applications folder, then the Utilities folder. Then, click the 'Terminal' application.

*FOR ADMIN PRIVILEGES:* <br> If you need admin privileges, start your command with 'sudo'. For example, `fakecommand --fake-option "some/fake/path"` would become `sudo fakecommand --fake-option "some/fake/path"`. You will be asked to enter your password, and then the command will run.

**Windows:**

Go to your 'Start Menu', then the' Windows PowerShell' folder, and click Windows PowerShell.

*FOR ADMIN PRIVILEGES:* If you need admin privileges, instead of left-clicking, **RIGHT-CLICK** the 'Windows PowerShell' application and Choose 'Launch as Administrator' (or something like that). Enter your password when prompted.

To learn the basics of command line, try the [free course at Codecademy](https://www.codecademy.com/)!

**END OF NOTE**

---

## 1 Python Interpreter

We will encounter Python, a very popular programming language. The 'English-like' appearance of the language makes it accessible to non-programmers. Nevertheless, it is very powerful and ideal for accomplishing many tasks in digital research.

I want to emphasize, you will not be required to master Python in this course. But, in order to understand digital research it helps to at least under the hood.

1. [Install Python 3.6](https://www.python.org/downloads/)

* Advanced OSX users, instead, follow [this guide](http://docs.python-guide.org/en/latest/starting/install3/osx/#install3-osx) which offers the best method to install

* During the course, you will attempt some of the lessons at [Codecademy's free Python Course](https://www.codecademy.com/learn/python). Feel free to check it out at your leisure.

---

## 2 GitHub Repository Manager

1. Install the [git-scm binary](https://git-scm.com/)
1. [Sign up for a GitHub Account](https://github.com)
2. [Install GitHub Desktop](https://desktop.github.com/)

* Advanced OSX Users, if you installed Homebrew in the Advanced step above, type `brew install git git-core` in the Terminal

---

## 3 Atom Text Editor

1. [Install Atom](https://atom.io/)
2. Configure Atom
    1. Either [follow this configuration guide](http://www.marinamele.com/install-and-configure-atom-editor-for-python)
    2. Or follow the TLDR summary below...

TLDR Summary:

1. Open your Terminal and enter the following...
``` shell
pip3 install flake8 flake8-pep257
apm install linter linter-flake8
```

2. Then restart Atom and click 'Hack on the Init Script' at the Welcome Guide, and paste the following on the last line...
``` coffee

process.env.PATH = ['/usr/local/bin/', process.env.PATH].join(':')
```

3. Then restart Atom, open the Preferences windows. Click the 'Editor' tab. Scroll down and Tab Length to 4 spaces and click Automatic PEP8 Validation

---

## 4 Slack Team Messenger

1. [Download and install](https://slack.com/downloads/) a copy of Slack messenger (or use their web interface)
2. Register an account at our course's Slack channel, [hacking-history.slack.com](https://hacking-history.slack.com/).

* For those interested, you can also register an account with the main Digital Humanities slack channel, [hacking-history.slack.com](https://digitalhumanities.slack.com/)

---

## 5 Tableau Visualization Platform

1. [Sign up for a student account](https://www.tableau.com/academic) (assuming you are a student), and then follow the instructions to install Tableau Desktop.
2. You will be able to use a 14-day trial, during which they will contact you with details for free access for a *full year.*

---

## 6 Google OpenRefine Data Scrubber

1. Head to [OpenRefine](http://openrefine.org/) and download the application.
2. You have to manually move the application to the location where you want to install it.

---

## 7 Trifacta Data Wrangler

*optional*

1. Head to [Trifacta](https://www.trifacta.com/start-wrangling/), register for a free account. Download the application, verify your email.
2. Start the Trifacta application and enter your account username and password

---
