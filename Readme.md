# GitHub Actions bug reproducer

This repository demonstrates an inconsistency in how conditionally skipped jobs are treated by the merge check algorithm.

* Jobs that do not run because of an `if` counts as "succeeded".
* Jobs that do not run because `path` directive counts as "failed".
