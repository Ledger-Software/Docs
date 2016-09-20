#Development Process

## Overview

The overall goal is to create a great product in the shortest amount of time.

## Commits To Master

All changes to master must go through pull requests. Also all changes to feature
branches that have more than one person working on them should be reviewed by the
other people working on that feature. If possible pull requests should be kept to
manageable sizes.

## Branchs

Master needs to always be in a releasable state. To ensure this each feature will be in
its own branch and each developer will commit to their own branch that is based on the
feature branch they are working on.

### Naming Example
* master
  * f_[Feature_Name]
    * f_[Feature_name]_[user]

## Code Review

All code needs to be reviewed by at least two people. Before a pull request is merged at least two people must approve the pull. If the pull request was pair programmed the one who did not post the pull request may count as one of the reviewers (still must
comment in the pull request).

### Puller

Give a general overview of what is included. For features give indication about the overall
progress of that feature that the pull request address.

State what type of feedback you want if it is not just general implementation and functionality checks.

The puller is also responsible for merging the branch once sufficient
reviews have been performed.

### Reviewer

Check to make sure what is stated as done is completed and that the merge will not adversely affect the base branch. Reviewers should check off their name on the
[Jira](http://cjm721.com:8080/secure/Dashboard.jspa) ticket once their review is complete and any issues have been addressed. Unless asked the review should be short and simple. See the following list of normal things to check for.

* Naming
  * Inconsistent Names
  * Ambiguous Names
  * Misleading Names
  * Long Names
*  Code
  * Duplicated / Repeated Code
  * Declared Assumptions
  * Coupling
* Tests
  * Adequate
  * All Passing

## Coding Standards

Readability is the main concern. In general [Google's Coding standard](https://google.github.io/styleguide/javaguide.html)
is a great resource but not required to be followed. Past that there is no required style.

All methods and structures should be named in a manner that gives simple info about what that element is for.

### Testing

**Code must be written so that it is testable.** All non-private methods should be have some form of unit tests (pure UI methods are the exception).
There should be Integration and System tests but those will be decided on a feature basis.

### WhiteSpace

There should be no tab character in any of the source code. It should be 4 spaces.
('\t' in strings is allowed)

### Documentation

All non-private methods and structures must have a JavaDoc element. Each element should be no longer
then a paragraph. If more is needed that is indicative that a refactor is needed or if explaining a design decision it can go into the implementation note.

## Agile Process

The team will use a scrum based process to aid in development. Sprints will be
one week long. Sprint retrospective and grooming will be held each Wednesday
after the meeting with the client. Stand-up meetings will be held each Monday,
Wednesday, and Friday. Monday meetings will be held at 5pm in one of the department's Computer Science labs. Wednesday meetings will be held at 2:30, and Friday meetings
will be held at 3:30. [Jira](http://cjm721.com:8080/secure/Dashboard.jspa) will be used to track the project's tasks.
