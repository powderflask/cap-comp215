# COMP 215: Intro. to Computational Science
Lessons, Labs, and Projects for COMP 215 Intro. to Computational Science at **Capilano University**

## Directory Structure

### labs
Starter notebooks for lab assignments

### lessons
In-class lessons, exercises, and reference material. <br>  
Weekly notebooks are used during class to structure discussion, answer questions,
and to demonstrate or test ideas that arose during class in a given week. <br>
Students should have a copy open and follow along during class.

foundations
: reference notebooks that review and demonstrate fundamental python programming concepts,
    algorithms, and data structures covered in the weekly lessons

concepts
: notebooks that explore the scientific concepts and models covered in the weekly lessons

algorithms
: reference notebooks that develop & present re-usable algorithms and/or data structures
that are re-used in the lessons, labs, or projects.

*Note*: for simplicity, rather than trying to `import` these as modules, 
         simply copy-paste what you need into the notebook you are working in.


## Branch Strategy

_Problem_
: retain term history in repo, ideally a branch for each semester.

  * keep it as simple as possible for students: reduce chance of mistakes; avoid merge conflicts
  * simplest for all if everyone just works in `default` branch

_Solution_
: use "release branch" strategy; work in "semester" release branch each term.

1. develop courseware, fix bugs in `main` branch
1. students work in `semester` branch, which is `default` branch and copy of `main` made at start of term.
1. post solutions and completed workbooks in `instructor` folder of `semester` branch 

_Process_

1. start of term:
    * create a `semester` branch from main (`git checkout -b 2024-Spr main`; `git push origin 2024-Spr`)
    * make the semester branch the `default` on GH
    * consider removing any solutions from previous term's branch to a private local branch
1. work in `semester` branch for production (current term):
    * students open lab assignments, exercises, and examples from `semester`
    * instructor posts completed workbooks and sample solutions to `instructor` folder on `semester` branch
    * careful not to update any notebooks in `semeseter` branch that might create merge conflicts for students
1. updating courseware during term:
    * fix bugs, enhancements, new lessons, etc. in `main` branch
    * advanced students can also make PR's to `main` branch
    * merge bug fixes back to `semester` branch only for notebooks not yet modified by students
    * students should always be able to update `semester` branch without conflict
1. end of term:
    * merge any changes you want to keep from `semester` branch back into `main` branch
