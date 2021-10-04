# Practy

Practy is an open-source collection of programming questions and exercises. The questions and exercises are sourced from textbooks, and they are ordered from basic to advanced.

Practy is written in markdown, deployed by MKDocs, and published on Github.

The goal of Practy is to provide a guided, hands-on learning experience by:

* Providing programming questions and answers from basic to advanced
* Providing programming exercises and solutions from basic to advanced
* Allowing developers to contribute to a beginner friendly open-source project

## Supported Languages

* Python
* JavaScript
* C#
* Java

## Using Practy

### Remote Dev Environment

[Visit Practy (dev)!](https://dev.d2w839m1wbzw.amplifyapp.com/)

### Install and Deploy Locally

Prequisites:

* Python 3
* Python Module: virtualenv

```bash

# Create a python virtual environment
python -m venv venv

# Activate the python virtual environment
. venv/bin/activate

# Upgrade Pip
pip install --upgrade pip

# Install Practy dependencies
pip install -r requirements.txt

# Deploy Practy
mkdocs serve
```

Open `http://127.0.0.1:8000/` in a browser
