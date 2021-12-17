# Refactoring Golf

    Refactoring Golf is a game designed to stretch your refactoring muscles and get you to explore your IDE to see what's really possible using shortcuts and automation.

    This repo contains several source trees, or numbered "Holes" based on a single exercise. Each hole carries on from the last for a single exercise - which is the application of a tax amount to a set of monatary amount.

    Your goal is to safely and efficiently as possible refactor the Hole-X code to look like the Hole X+1 code. You must aim to do it in as few "strokes" as possible.

    A "stroke" is essentially a change made to the code, and every stroke costs you points.

    Your pairing partner should carefully score you as follows:

      - 1 point for every change made to the code using a shortcut or automated IDE feature (e.g., an automated refactoring, code template, or Find/Replace)
- 2 points for every manual edit. Note that a single "edit" could cover multiple lines of code.
- Double points for every change made while the code cannot pass the tests after the previous change.
- Zero points for code formatting (e.g., deleting whitespace or optimizing imports).

Allow yourselves a maximum of 2 attempts at each round to determine your best score.

## Hints: 

1. You may find that customising your IDE is useful (e.g. custom code templates, or even custom refactorings.)

2. If possible, it would be a good idea to have the two versions (Hole X and Hole X+1) of each set of source files open on different machines, as you could easily tie yourself in knots editing the wrong files!

3. Keep that second machine available as a tooling environment. Writing custom tools (scripts, templates etc) costs you zero points in refactoring golf.

## Course records:
These are the best known scores, achieved using IntelliJ:

| Hole | Best score | Notes | My score |
|------|------------|-------|----------|
| 1    | 3          |   4   | 1 (To Equals call) + 1 (To Equals call) + 1 (Invert if) + 1 (Remove redundant else)        |
| 2    | 7          |   7   | 1 (rename param) + 1 (rename param) + 1 (change signature) + 1x2 (change type) + 1x2 (remove redundant type)         |
| 3    | 5          |   7   | 2 (merge foreachs) + 1 (extract method) + 1 (make method non-static) + 1 (rename parameter) + 1 (inline return) + 1 (inline variable  )   |
| 4    | 6          |   7   | 1 (extract method) + 1 (make method non-static) + 1 (delete param) + 2 manual fix param + 1 factory method + 1 remane param   |
| 5    | 10         |   9   | 1 (extract class) + 1 (introduce param in ctor) + 1 (extract method Apply) + 2 (change use of first -> total) + 1 (safe dalete first param) + 1 (inline return) + 1 (move instace method) + 1 (factory method)  |
| 6    | 7          |   6   | 1 (convert to linq) + 1 (inline variable) + 2 (manually remove ToList) + 1x2 (raname lambda variables)     |
 
**My total: 44**

<b>Course Record: 38</b>

## Acknowledgements:
This exercise was developed with Ivan (@s4nchez). :)
Thanks to @ivanmoore and @rchatley for the inspiration.
These instructions were mostly stolen from @jasongorman's <a href="https://github.com/jasongorman/RefactoringGolfJava">Refactoring Golf repo</a>
