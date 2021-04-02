### Code Reviews
#### Into
***

Agile teams are self-organizing, with skill sets that span across the team.
This is accomplished, in part, with code review.
Code review helps developers learn the code base, as well as help them learn
new technologies and techniques that grow their skill sets

#### What is a code review?
***
Code review is a circular process on a specific branch before it reaches the merge phase into the dev or master branch.
Code reviews are done when a developer makes a pull request.

The process starts when the branch owner (the developer) finishes work on a feature and makes a pull request, where he
sets the destination branch for future merging. They then tag either the entire team, part of the team (usually, the
ones who are specialized in that programming language if the project is developed using multiple languages), or a single
person who can be the team lead, solutions engineer or a senior member of the team.

The reviewers are usually selected at the start of the project, and they remain until the project is finished.

#### How does it work?

***
Usually only one of the tagged reviewers will perform the code review. When performing code reviews, we use the
following process:

* Are there any obvious logic errors in the code?
* Looking at the requirements, are all cases fully implemented?
* Does the new code conform to existing style guidelines?
* Does the new code fix the problem?
* It is the code legible, can it be written in a more simplified way?
* Are the new automated tests sufficient for the new code?

With the above questions in mind, the reviewer starts analyzing the code and leaves comments if any of the above issues
are present, so the branch owner can fix the problem. The branch owner will read the comments and will fix or try to fix
the highlighted issues. This process will be repeated until all the problems are fixed.

When everything is fixed, the reviewer will approve the pull request. After the approval, the code will be merged into
dev. Feature branches are merged in the dev branch, eventually all of those merges form a "code package" which usually
goes in master.

Before merging to master, the "code package" is deployed on a staging server to make sure everything is working
normally.

If everything is ok on the staging server, the package is merged into master, then the deployment process is next, where
the "package code" is deployed on the server from the master branch.

#### References

***
[Why code reviews matter ](https://www.atlassian.com/agile/software-development/code-reviews)

[Gabriel Cliseru - Senior QA](https://github.com/settlersxp) on [deindeal](https://www.deindeal.ch/)
