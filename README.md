# Problem Solving with Python — Chapter 16: Catch Them Early

This repository contains the chapter and active-learning exercise code associated with this chapter in the book *Problem Solving with Python: Using Computational Thinking in Everyday Life* by Michael D. Smith (2026), which is available from [MIT Press](https://mitpress.mit.edu/9780262383677/problem-solving-with-python/) and [Amazon](https://www.amazon.com/Problem-Solving-Python-Computational-Thinking/dp/0262552841/).

## Getting started

You will need:

- an integrated development environment (IDE)
- Python 3.10 or newer
- `pip` (usually included with Python)

If you need help getting started with an IDE, please read [my short introduction to "Understanding and Selecting an IDE"](https://ctps.io/select_ide.html).

## Cloning this repository

If you're using GitHub Codespaces, click the green "Code" button on this repo's page, select the tab "Codespaces," and click the "Create codespace on main."

Otherwise, in your IDE's terminal window, type the following commands:

```bash
git clone https://github.com/pswp-book/chap16.git
cd chap16
```

## (Optional) Create and activate a virtual environment

```bash
python -m venv .venv
# Windows
.\.venv\Scripts\activate
# macOS/Linux
source .venv/bin/activate
```

## Install dependencies

```bash
pip install -r requirements.txt
```

If there is no file `requirements.txt`, the code in this repository uses only the Python standard library.

## Reporting issues

If you find a problem in this chapter’s code (typo, bug, or mismatch with the book):

1.  Check the issues for this repo to see if it’s already reported.

2.  Open a new issue and include:
    *   The chapter number and section title (e.g., “Chapter 5, The game loop”)
    *   The filename, line number(s), and a short description of the problem.
    *   If something's wrong with the code's execution, please describe how you ran the program and the exeuction result.

## Short description of the repo's files

`bookshelf1-anno.py`: A copy of `bookshelf1.py` from Chapter 3 with the addition of type hints, which demonstrates that difficulty of using type hints and data abstraction. The problem is that not all sequence types in Python support concatenation. Enable mypy to see the type errors.

`dbzero.py`: A simple script containing an obvious divide-by-zero error.

`dbzero1.py`: A slightly more complicated script containing a divide-by-zero error.

`dbzero2.py`: A script that sometimes raises a divide-by-zero runtime error.

`dbzero3.[py,c]`: Code that illustrates the difference between interpretation and compilation.

`dyntype.py`: A simple example of dynamic typing and how easy it is to not know statically the type of the object in a name.

`emdash.py`: A script that allows a user to indicate which parenthetical phrase should be offset with em dashes rather than commas. It contains a silly coding bug.

`emdash-anno.py`: The `emdash.py` script with type hints that allow mypy to find the type error.

`emdash-fixed.py`: The `emdash.py` script with the type error corrected. Don't peek!

`equal.py`: A short script showing that two objects with the same value expressed as bits are not considered equal by Python.

`equal.c`: A C-language-version of `equal.py` showing that C doesn't consider type information at runtime.

`equal2.c`: Another version of `equal.c` with the variable declaration separated from the variable initialization.

`fun.c`: A simple C program used to demonstrate compiling to an executable.

`txts/debugging.txt`: Input used in `emdash.py` example.
