## Code Reviews
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

***

### Some extra Guidelines for Code Reviews

When we review code, we should look at it as a process that can be continually improved rather than a set of unchanging commandments. With that in mind we have some extra guidelines that people should be aware of when making reviews.

#### Tone of review
Maintain a professional tone and keep any comments constructive and related to the code; 'Play the ball, not the person'. Give comments that include suggestions rather than saying something like 'this is incorrect'. When reviewing, avoid having the mindset of it's wrong because it's not the way I would do it; instead try to review the code on whether it is correct.

#### Reviewing new joiners code
Do not change the standard process outlined in the 'How does it work?' section above but be mindful that the person may
not be aware of the coding standards or may be not be totally up to speed with the codebase. The above section is never
more important than when reviewing a new joiners code.

#### Your part as a Reviewee
Don't take someone not approving your PR or suggesting changes as a personal attack. It's part of the process of software development and it helps everyone learn, improve, makes for a more open team culture and ensures quality code: 
> "**The biggest thing that makes Google’s code so good is simple: code review.**" Mark Chu-Carroll

Code reviews should not be a daunting prospect but an opportunity to gain valuable feedback and improve your performance.

#### References
Title | Author | Link
------------ | ------------- | -------------
How to Make Good Code Reviews Better | Gergely Orosz | [Article Link](https://stackoverflow.blog/2019/09/30/how-to-make-good-code-reviews-better/)
Lessons from Google: How code reviews build company culture | Bruce Johnson | [Article Link](https://www.fullstory.com/blog/what-we-learned-from-google-code-reviews-arent-just-for-catching-bugs)
Things Everyone Should Do: Code Review | Mark Chu-Carroll| [Article Link](http://www.goodmath.org/blog/2011/07/06/things-everyone-should-do-code-review/)
The value of code reviews in an engineering team | John Doran | [Article Link](https://nothingventured.rocks/the-value-of-code-reviews-in-an-engineering-team-ab1482d26717)
Why code reviews matter (and actually save time!) | Dan Radigan | [Why code reviews matter ](https://www.atlassian.com/agile/software-development/code-reviews)
Personal experience about Code Review | Gabriel Cliseru | [Gabriel Cliseru - Senior QA](https://github.com/settlersxp) on [deindeal](https://www.deindeal.ch/)

