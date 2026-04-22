# GitExercise_Conflicts

1. Clone this repo to your datahub or local computer (your choice)
1. Merging ex1 branch into main branch... the difference here is a simple line of text conflict\\
   1. first look at the diff
   1. now merge e1 into main; note how the conflict gets shown to you...
   1. resolve the conflict in whichever way you choose,
   1. add and commit the changes on main
1. Merging ex2 branch into main branch... the difference here is metadata and binaries from a plot
   1. first look at the diff
   1. now checkout e2.
   1.  remove the metadata and outputs by clearing all cell output
   1. add and commit the changes on e2
   1. now merge e2 into main
   1. resolve the conflict in whichever way you choose,
   1. add and commit the changes on main
# GitExercise_Conflicts

This exercise assumes you are using the COGS 108 Datahub setup. But you can do everything here using your own computer if you set it up with the same tools.

## Purpose
To teach you to deal with git merge conflicts in:
- Jupyter Notebooks
- Datahub using graphical tools

## Problem overview

This repo contains two branches: main and ex1. There is a single line text conflict in one cell between the two branches.

Below is a graph of the commit situation:

----*----*[main]
     \
      \----*[ex1]

We will do two operations:
- Part 1: add a change to main
- Part 2: merge ex1 into main

After Part 1:
----*----*----*[main]

After Part 2:
----*----*----*----*[main]
     \             /
      \----*------/