# <center>Software Quality Guidebook</center>
## Introduction
The purpose of this handbook is to provide a resource that people can reference for the following topics: 

-	Task estimation in Scrum
-	Coding standards
-	Code reviews

### Content
***
- Task Estimation in Scrum
	- Introduction
	- How it is done

- Coding standards
	- Importance of Coding Standards
	- Formatting
	- Naming Conventions
	- Version Control
	- Comments
	- Classes and Functions
	- Testing

- Code Reviews
    - Introduction
    - What is a code review?
    - How does is work?
    - Extra Guidelines


### Task estimation in Scrum
#### Introduction
***
Task estimation is a team sport. Everyone (developers, designers, testers, management people) from
the team has to be involved, it is the key to succeed in one of the difficult aspects of the job.

Usually once every week or two weeks the whole team gather together to start planning the next sprint.
Each sprint has a goal, and to achieve that goal, certain stories has to be created, velocity and burndown
chars has to be analyzed in order to achieve that goal.

#### How it is been done
***
The main part of a sprint are the user stories. Story is divided in tasks and typically is a functionality
that will be visible to end users. It represents something that generally is worked on by more than one person.

Tasks on the other hand, is typically something like "code this", "design that", "create test data for" and so on.
Tasks tend to be things done by one person.

When the estimation starts usually are two outcomes.
1. Story complexity which is something common between all team members.
2. Work hours per Task from the Story, which is an average between the people who work on a specific technology.

When, "work hours" are estimated there are big chances that the estimation is not close to a real scenario.


The main reason is that most of the time developers ignore certain steps from a completed task. A
task is considered complete when is "delivered", in other words developed, tested, merged and deployed.
When developers estimate they consider only the developing part and sometimes the testing part but they
forget to estimate things like.

+ The task may come back to them for certain fixes.
+ Solving the Git conflicts
+ Unexpected bugs.
+ Integration issues.

The best estimation are given by the QA people. They take into consideration the development time given
by the developers and on top of that they add time for testing and bugs because they are familiar with
this kind of situations and at the end something close to the truth is given.


#### Benefits & Challenges Task Estimation :
***
     **Benefits**

        The advantages that can be leveraged through task estimation can laid out as follows :
        1. Allows an insight into the uncertainty of a project
        2. Allows the team to rejudge the project as they understand the project as time progresses reducing uncertainty
        3. Estimates become more reliable which leads to a better deliverable and relationships strengthen between all parts
        4. Estimation supports the decision makers by providing insight the worst and time frame of the project

&nbsp;

#### Challenges
***
Even though, as discussed in the preceding points, task estimation is useful in project planning. These are some of the difficulties that people who are in control of task estimation face : 1. Nuance between estimates and commitments. 2. Features are not prioritised and there is no structure in how they are built out. 3. The ambiguity is often ignored. 4. The time frame is often based on the competition of activities over features.

#### Taking on the challenges
***


Using agile planning techniques, we can overcome difficulties in the task estimation phase in scrum. + Work can be done in iterations, this allows a set of requirements to be broken down into features that are finished. Seperaretly planning is done through iterations too.

- Features are prioritised for release, so user stories can be delivered first. Conditions for success at feature and project level are drawn up so that the aims of the iterations are clear.
- Plans are always being updated as the knowledge is gained and so too are the priorities.
- The backlog will not give an estimation for the project.
- Any issue faced should not be picked randomly from the backlog.


#### Building out a successful story point estimation
***


In sizing, the team does an analysis between the different stories for the project. Every story to be sized the following needs to be done, from the PO, developers and Scrum master:

1. Identify stories
2. Discuss the requirements of the story.
3. Take notes for what you want when building the story
4. Find relative sized points for comparison or previous tasks.
5. Conclude as a team about the sizes of the stories.
6. Confirm that your estimates are consistent as the stories progess.
7. Reasses that the indentified stories match the requirements.

| Advantages                                          | Disadvantages                                                   |
| --------------------------------------------------- | --------------------------------------------------------------- |
| Greater control over sprint                         | Overheads with no inherit value can affect accuracy of estimate |
| More accurate estimates                             | Hours worked combined with logging hours                        |
| Harder to under or over comit                       | Working In Hours May Lead To Micro-Managing                     |
| Unfinished work is clear to see                     |                                                                 |
| Input is can be giving after the fact and is valued |                                                                 |

#### Bad practices of Task Estimation
***


    + Teams can be interrupted when in production or other responsibilties arise.
    + Teams give estimates with out regard for skill level and experience.
    + Teams sometimes have memebers join and leave and this can affect the productivity.

#### References
***
Title | Link
------------ | -------------
User Stories with Examples and Template |  [Article Link](https://www.atlassian.com/agile/project-management/user-stories#:~:text=A%20user%20story%20is%20the,work%20in%20an%20agile%20framework.&text=Stories%20fit%20neatly%20into%20agile,run%20them%20through%20their%20workflow)

The Difference Between a Story and a Task |  [Article Link](https://www.mountaingoatsoftware.com/blog/the-difference-between-a-story-and-a-task#:~:text=A%20story%20is%20something%20that,on%20by%20just%20one%20person.&text=A%20task%2C%20on%20the%20other,things%20done%20by%20one%20person)

Agile Planning and Estimation |  [Article Link](https://www.oreilly.com/library/view/head-first-agile/9781491944684/ch04.html)

Gabriel Cliseru - Senior QA |  [Article Link](https://github.com/settlersxp) [deindeal](https://www.deindeal.ch/)

A beginners guide to agile estimation and planning | [Article Link](https://endjin.com/blog/2019/02/a-beginners-guide-to-agile-estimation-and-planning)

Agile Estimation Challenges | [Article Link](https://blog.valuemotive.com/agile-estimation-challenges-636184e8b199)

Why estimate in Scrum | [Article Link](https://maartendalmijn.com/why-estimate-twice-in-scrum-fd0d68744501)

Why your agile teams are bad at estimation | [Article Link](https://www.linkedin.com/pulse/why-your-agile-teams-bad-estimation-heidi-araya)


### Coding Standards
***
Coding standards are collections of rules and guidelines that determine the programming style, procedures, and methods for a programming language.

#### Importance of Coding Standards
***
Without coding standards, every individual in a team will use their own coding styles. 
It will not be easy to maintain and will be difficult to debug the code.

#### Formatting
***
Code formatting allows programmers to vaguely convey what their code intends to do. 
Code formatting is often a programmer's reader's first encounter with their system. 
It deserves attention and care.

#### Components That Affect Code Formatting:
***
* Quick Readability: The reader should be able to understand the gross structure of the code in a glimpse. 
  The shapes made by blocks of text help you communicate the overall structure.

* Detailed Readability: The reader must be able to read lots of code in depth.

* Length: The number of lines must be minimized so that browsers can be as small as possible.

* Width: The width of code must be minimized. Code must not ordinarily spill across the right margin, 
  requiring horizontal scrolling or destroying the shape of the text with line wrapping.

#### Essential Parts of Code Formatting
***
Conventions have been made to make sure code is as understandable as possible. 
This helps avoid errors, troubleshoot problems and makes maintaining someone else’s (or even your own) work much easier.

There are differing conventions depending on the language that you are using. 
Yet, all of them basically revolve around the following:

1. Indentation 
2. White space
3. Capitalization and naming conventions
4. Style and spelling of functions, variables and more
5. Use and style of comments

#### Naming Conventions
***
 A naming convention is a set of rules for choosing the character sequence to be used for identifiers 
 which represent variables, types, functions, and other entities in source code and documentation.

#### Significance of Naming Conventions
***
It is important for programmers to utilise and agree on naming conventions instead of allowing everyone
to choose any character sequence.

The following are reasons why: 

* To reduce the effort needed to read and understand source code
* To enable code reviews to focus on more important issues than arguing over syntax and naming standards.
* To enable code quality review tools to focus their reporting mainly on significant issues other than syntax and style preferences.

#### Potential Benefits 
***
Some of the potential benefits that can be obtained include the following:

* to help formalise expectations and encourage consistency within a development team;
* to enable the use of automated refactoring or search and replace tools with minimal potential for error;
* to enhance clarity in cases of potential ambiguity;
* to help avoid "naming collisions" that might occur when the work product of different organisations is combined.
* to provide meaningful data to be used in project handovers which require submission of program source code and all relevant documentation;
* to provide better understanding in case of code reuse after a long interval of time.

#### Version Control
***
* For each new task, a feature branch should be checked out from the development branch.
* The new branch name should be based off the task e.g. task is check correct email input, branch name could be check-email-input.
* Pull requests require at least two approvals before merge.
* Click [here](https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet) for a Git command cheat sheet

#### Comments
***
For comments, we subscribe to the idea that if the code should be explanatory. If it needs comments, then it is poorly thought out either in terms of naming or the code itself being overly complicated so it cannot be easily understood.

Commented out code should never be allowed be part of the code. If it's commented out; it should not be there.

### Classes and Functions
***
#### Classes
***
Try to maintain small classes, ensuring that they have one responsibility rather than creating a "God class".

#### Functions
***
Functions should be short and have a singular purpose. We strive to make sure that:
> **Functions should do one thing. They should do it well. They should do it only.**
> Robert C Martin - Clean Code

Avoid excessive number of arguments in your functions. Try to ensure there are no side effects.
Follow the 'don't repeat yourself' principle (DRY). Duplication bloats code and is inefficient.

#### Testing
***
For any changes code or new code, write unit tests! For testing we use the Arrange-Act-Assert pattern:
```
     @Test                                               
	    public void testAdd() {
		 //Arrange
		 int expected = 12;
         //Act
		 int actual = calculator.add(9, 3);
         //Assert
		 assertEquals(expected, actual);         
	    }
```
Although this example is in Java, unit tests in other languages should follow this pattern.
While the comments contradict the earlier instructions, they are for demonstrative purposes only!

#### References
***
Title | Link
------------ | -------------
Clean Code  | [Authors Website](http://cleancoder.com/products)
7 key coding practices for agile developers | [Article Link](https://www.infoworldcom/article/3446439/7-key-coding-practices-for-agile-developers.html)
How to write clean code? | [Article Link](https://medium.com/mindorks/how-to-write-clean-code-lessons-learnt-from-the-clean-code-robert-c-martin-9ffc7aef870c)
Coding Standards and Conventions in Software Development Teams| Prince Sengayire |[Article Link]( https://medium.com/@psengayire/the-importance-of-coding-standards-and-conventions-in-the-software-development-team-how-they-can-5d252556a05#:~:text=Coding%20standards%20are%20collections%20of,methods%20for%20a%20programming%20language.&text=Without%20the%20coding%20conventions%2C%20every,code%20in%20the%20near%20future.)
ARRANGE-ACT-ASSERT: A PATTERN FOR WRITING GOOD TESTS |  [Article link](https://automationpanda.com/2020/07/07/arrange-act-assert-a-pattern-for-writing-good-tests/)
Gitflow Workflow | [Tutorial Link](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow#:~:text=The%20overall%20flow%20of%20Gitflow,branch%20is%20created%20from%20master&text=When%20the%20release%20branch%20is,to%20both%20develop%20and%20master)
Code Formatting Guide | [Article Link](https://torquemag.io/2019/07/code-formatting-guide/)
Java Style Guide |  [Article Link](https://google.github.io/styleguide/javaguide.html#s4-formatting)
Code Formatting Patterns |  [Article Link](http://c2.com/ppr/formatting.html#6)
Naming Conventions | [Article Link](https://en.wikipedia.org/wiki/Naming_convention_(programming)#:~:text=In%20computer%20programming%2C%20a%20naming,in%20source%20code%20and%20documentation)



### Code Reviews
#### Intro
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


#### Some extra Guidelines for Code Reviews
***
When we review code, we should look at it as a process that can be continually improved rather than a set of unchanging commandments. With that in mind we have some extra guidelines that people should be aware of when making reviews.

#### Tone of review
***
Maintain a professional tone and keep any comments constructive and related to the code; 'Play the ball, not the person'. Give comments that include suggestions rather than saying something like 'this is incorrect'. When reviewing, avoid having the mindset of it's wrong because it's not the way I would do it; instead try to review the code on whether it is correct.

#### Reviewing new joiners code
***
Do not change the standard process outlined in the 'How does it work?' section above but be mindful that the person may
not be aware of the coding standards or may be not be totally up to speed with the codebase. The above section is never
more important than when reviewing a new joiners code.

#### Your part as a Reviewee
***
Don't take someone not approving your PR or suggesting changes as a personal attack. It's part of the process of software development and it helps everyone learn, improve, makes for a more open team culture and ensures quality code: 
> "**The biggest thing that makes Google’s code so good is simple: code review.**" Mark Chu-Carroll

Code reviews should not be a daunting prospect but an opportunity to gain valuable feedback and improve your performance.

#### Purpose & Benefits of Code Reviews:
***

* Allows developers to detect bugs early in the code.
* Improving code for better performance. Developers are able to identify 
  areas where they can improve their code. Members can learn code optimisation
  techniques from each other that can help them write clean code.
* Code reviews is a coding standards compliance. 
  It allows developers to maintain consistent coding style.
* Enables everyone to teach and share information and knowledge. 
  Team members are able to gain a better understanding of the code 
  base and learn from each other during reviews.
* Consistent design and implementation. 
  Code reviews helps us maintain a level of consistency in 
  software design and implementation.
* Team solidarity. Team members are able to bond and become closer 
  to each other when they review and discuss each other's code. 
  Allows them to become more comfortable with each other and the code they produce.

#### References
***
Title | Link
------------ | ------------- | -------------
How to Make Good Code Reviews Better |  [Article Link](https://stackoverflow.blog/2019/09/30/how-to-make-good-code-reviews-better/)
Lessons from Google: How code reviews build company culture | Bruce Johnson | [Article Link](https://www.fullstory.com/blog/what-we-learned-from-google-code-reviews-arent-just-for-catching-bugs)
Things Everyone Should Do: Code Review |  [Article Link](http://www.goodmath.org/blog/2011/07/06/things-everyone-should-do-code-review/)
The value of code reviews in an engineering team |  [Article Link](https://nothingventured.rocks/the-value-of-code-reviews-in-an-engineering-team-ab1482d26717)
Why code reviews matter (and actually save time!) |  [Why code reviews matter ](https://www.atlassian.com/agile/software-development/code-reviews)
Personal experience about Code Review |  [Gabriel Cliseru - Senior QA](https://github.com/settlersxp) on [deindeal](https://www.deindeal.ch/)
Understanding Code Review and its Benefits | [Article Link](https://www.browserstack.com/guide/code-review-benefits)

