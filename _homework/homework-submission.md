---
layout: guides
navbar: Guides
title: Homework Submission
key: 3
---

This guide discusses the homework submission process. This comes *after* the [Homework Setup](homework-setup.html) and [Homework Testing](homework-testing.html) processes.

## Submission

To submit your homework, make sure the latest version of your code has been committed **and** pushed to Github. There are two things to verify:

  1. Make sure you see your latest commit when visiting the homework repository on the Github website.

  2. Make sure you are passing all of the tests when running the `homework` script on the lab computers. (See [Homework Testing](homework-testing.html) for details.)

We use the `homework` script on the lab computers for grading, so if that is passing the tests then it will pass the tests when we grade it as well.

Otherwise, there is nothing else to do to submit your homework. We will use Github Classroom to get a list of all the repositories and grade them automatically.

## Late Policy

Partial grades are not given for homework assignments; students must pass 100% of the provided tests to earn credit. If all of those tests pass before the deadline, the student will earn a 100% on that homework assignment.

Otherwise, there will be a **–5% deduction per day** (24 hours) the homework is late based on the commit timestamp of the repository. **Homework will not be accepted if it is more than one week late.**{: .has-text-danger }

#### Avoiding the Late Penalty

Want to keep working on your homework after the deadline? No problem; just [create a branch](/guides/general/using-branches.html) of your homework first! This avoids making any modifications to your `master` branch, allowing you to avoid the automatic late penalty. If you are able to get additional tests passing, you can merge those changes back into your `master` branch.

See the [Using Branches](/guides/general/using-branches.html) guide for details on this process.

#### Contesting the Late Penalty

Mistakes still happen. You can contest the automatic late penalty if you accidentally change the timestamp of your `master` branch, but were fully passing the tests *before* the deadline.

This is only possible if you have a commit in your repository before the deadline that was passing the tests. We will be able to check out that exact commit and verify the test results.

You get one free warning without penalty. If you make this mistake more than once, you will lose a 5% submission penalty for each additional offense.
