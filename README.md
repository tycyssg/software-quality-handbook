### Code Reviews
#### Into
***

Agile teams are self-organizing, with skill sets that span across the team.
This is accomplished, in part, with code review.
Code review helps developers learn the code base, as well as help them learn
new technologies and techniques that grow their skill sets

#### What is code review
***
Code review is a circular process on a specific branch before it reaches the merge phase into dev
or master.
The place where the code review is being done is the pull request.

The process starts when the branch owner (the developer) finish the job and make a pull request, where
he sets the destination branch for future merging and tag either the entire team, part of the team
(usually, the ones who are specialized in that programming language) in case the project is developed
based on multiple languages, or a single person who can be the team lead, solutions engineer from or
a senior from the team.

#### How it works?
***
From the whole tagged persons most of the time only one will perform the code review. The reviewer,
in the process, will consider questions like:
* Are there any obvious logic errors in the code?
* Looking at the requirements, are all cases fully implemented?
* Does the new code conform to existing style guidelines?
* Does the new code fix the problem?
* It is the code legible, can be written in another simplified way?
* Are the new automated tests sufficient for the new code?

With the above questions in mind, the reviewer start analyzing the code and leave comments if is the case
exactly on the code line for better visualization of the branch owner when this one has to fix the problem.

The branch owner will read the comments and will fix or try to fix the exposed issues. This process
will be repeated until all the problems are fixed.

When everything is fixed, the reviewer will approve the pull request. After the approval, the code will be
merged into dev. In the dev branch are merged all others branches, and from time to time all of those merges form a "code package" which usually goes in master. Before going in master, the "code package" is deployed on a
staging server to make sure everything is working normally.

If everything is ok on the staging server, the package is merged into master, then the deployment process is next, where
the "package code" reaches the server from the master branch.
