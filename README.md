# Practy

Practy is an open-source collection of programming questions and exercises. The questions and exercises are sourced from textbooks, and they are ordered from basic to advanced.

Practy is written in markdown, deployed by MKDocs, and published on Github. It currently supports exercises in Python and JavaScript.

The goal of Practy is to provide a guided, hands-on learning experience by:

* Providing programming questions and answers from basic to advanced
* Providing programming exercises and solutions from basic to advanced
* Allowing developers to contribute to a beginner friendly open-source project

## Supported Languages

* python
* javascript

## Installation and Deployment

Prequisites:

* Python 3
* Python Module: virtualenv

```bash
python -m venv venv

. venv/bin/activate

pip install --upgrade pip

pip install -r requirements.txt

mkdocs serve
```

Open `http://127.0.0.1:8000/` in a browser
