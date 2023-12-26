# COMP 215: Intro. to Computational Science
Exercises, Labs, and Projects for COMP 215 Intro. to Computational Science at **Capilano University**

## Directory Structure

### examples
Complete notebooks used in-class to demonstrate principles

### exercises
Starter notebooks used in-class as a starting point for group exercises and practice problems

### labs
Starter notebooks for lab assignments

### weekly
Notebooks used during class to answer questions and test ideas that arose during class in a given week

## Branch Strategy
_Problem_
:  students will not remember to load content from a branch - so use `main` as "production" version

_Solution_
: use a "release branch" strategy to save semester's work at end of term and re-use `main`  over successive terms.

1. fork this repository
2. create a `template` branch (save a copy of the original codebase as a template)
3. work in `main` branch, students open lab assignments, exercises, and examples from `main`
4. end of term, create a branch from `main` named for the term (e.g., `2023-Spring`) to backup work
5. merge any changes you want to keep back into `template` branch
6. override `main` with fresh copy of `template`, ready for next term