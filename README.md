# COMP 215: Intro. to Computational Science
Exercises, Labs, and Projects for COMP 215 Intro. to Computational Science at **Capilano University**

## Directory Structure

### labs
Starter notebooks for lab assignments

### lessons
In-class lessons, examples, and reference material. <br>  
Weekly notebooks are used during class to structure discussion, answer questions,
and to demonstrate or test ideas that arose during class in a given week. <br>
Students should have a copy open and follow along during class.

foundations
: reference notebooks that review and demonstrate fundamental python programming concepts,
  and built-in functions & data structures covered in the weekly lessons

concepts
: notebooks that elaborate on the scientific concepts and models covered in the weekly lessons

algorithms
: library notebooks that develop & present a re-usable algorithm and/or data structure
that is used in the lessons, labs, or projects.

*Note*: for simplicity, rather than trying to `import` these as modules, 
         simply copy-paste what you need into the notebook you are working in.

exercises
: starter notebooks for in-class exercises and practice problems


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