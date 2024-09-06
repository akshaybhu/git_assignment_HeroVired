# CalculatorPlus 


## Baseline scenario:

The application provides basic arithmetic operations, such as addition, subtraction, multiplication, and division. Our task is to implement a new feature that adds support for calculating the square root of a number under a new branch called ‘feature/sqrt’.

## Critical Bug Fix

The bug fixation is in the divide function for "Cannot divide by zero", so in case someone enters divisor as 0 we should have a exception rather than breaking the whole scirpt.
Due to this bug, we had to halt the sqrt feature and fix this bug prior.

After fixing the bug, we saw merge conflicts as the changes were in same file. 

## Resolution

I resolved the bug using Github user interface, by reviewing lines under conflict, view last merged PR with exact changes and remove unwanted branch info/lines.





======================================================================================================




# Geometry-Calculator


## Baseline scenario:

Defined simple class using Python program that calculates the area of a circle and the area of a rectangle. We used Git stash/Git stash apply to manage multiple branch changes simultaneously.


## Simultaneously work on 2 branches

1) "feature/circle-area" to work on the circle area feature.
2) "feature/rectangle-area" to work on the rectangle area.


## Issue Faced

On branch "feature/circle-area", I first created all changes but performed git stash to save all changes on that particular branch only tmeporarily.
Moved to create new branch "feature/rectangle-area", and once changes were prepared, I used git stash to save changes on that particular branch only tmeporarily again.

Now once back to branch "feature/circle-area", i used git stash apply to move the branch in time to apply respective changes and performed git add/commit/push.
Same goes for branch "feature/rectangle-area" and performed same sequence.

Lastly, on merging 1st branch "feature/circle-area" we could see merge conflicts on 2nd branch "feature/rectangle-area" and resolved the same using Github interface and as per structured code to perform correct are calculations.

