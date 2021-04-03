# Introduction
The purpose of this handbook is to provide a resource that people can reference for the following topics: 

-	Task estimation in Scrum
-	Coding standards
-	Code reviews

### Content

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
#### Intro
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


#### References
***
[Story points and estimation](https://www.atlassian.com/agile/project-management/estimation)

[User Stories with Examples and Template](https://www.atlassian.com/agile/project-management/user-stories#:~:text=A%20user%20story%20is%20the,work%20in%20an%20agile%20framework.&text=Stories%20fit%20neatly%20into%20agile,run%20them%20through%20their%20workflow)

[The Difference Between a Story and a Task](https://www.mountaingoatsoftware.com/blog/the-difference-between-a-story-and-a-task#:~:text=A%20story%20is%20something%20that,on%20by%20just%20one%20person.&text=A%20task%2C%20on%20the%20other,things%20done%20by%20one%20person)

[Agile Planning and Estimation](https://www.oreilly.com/library/view/head-first-agile/9781491944684/ch04.html)

[Gabriel Cliseru - Senior QA](https://github.com/settlersxp) on [deindeal](https://www.deindeal.ch/)



# Coding Standards

Coding standards are collections of rules and guidelines that determine the programming style, procedures, and methods for a programming language.

### Importance of Coding Standards

Without coding standards, every individual in a team will use their own coding styles. 
It will not be easy to maintain and will be difficult to debug the code.

## Formatting

Code formatting allows programmers to vaguely convey what their code intends to do. 
Code formatting is often a programmer's reader's first encounter with their system. 
It deserves attention and care.

### Components That Affect Code Formatting:

* Quick Readability: The reader should be able to understand the gross structure of the code in a glimpse. 
  The shapes made by blocks of text help you communicate the overall structure.

* Detailed Readability: The reader must be able to read lots of code in depth.

* Length: The number of lines must be minimized so that browsers can be as small as possible.

* Width: The width of code must be minimized. Code must not ordinarily spill across the right margin, 
  requiring horizontal scrolling or destroying the shape of the text with line wrapping.

### Essential Parts of Code Formatting

Conventions have been made to make sure code is as understandable as possible. 
This helps avoid errors, troubleshoot problems and makes maintaining someone else’s (or even your own) work much easier.

There are differing conventions depending on the language that you are using. 
Yet, all of them basically revolve around the following:

1. Indentation 
2. White space
3. Capitalization and naming conventions
4. Style and spelling of functions, variables and more
5. Use and style of comments

## Naming Conventions

 A naming convention is a set of rules for choosing the character sequence to be used for identifiers 
 which represent variables, types, functions, and other entities in source code and documentation.

### Significance of Naming Conventions

It is important for programmers to utilise and agree on naming conventions instead of allowing everyone
to choose any character sequence.

The following are reasons why: 

* To reduce the effort needed to read and understand source code
* To enable code reviews to focus on more important issues than arguing over syntax and naming standards.
* To enable code quality review tools to focus their reporting mainly on significant issues other than syntax and style preferences.

### Potential Benefits 

Some of the potential benefits that can be obtained include the following:

* to help formalise expectations and encourage consistency within a development team;
* to enable the use of automated refactoring or search and replace tools with minimal potential for error;
* to enhance clarity in cases of potential ambiguity;
* to help avoid "naming collisions" that might occur when the work product of different organisations is combined.
* to provide meaningful data to be used in project handovers which require submission of program source code and all relevant documentation;
* to provide better understanding in case of code reuse after a long interval of time.

## References



## Version Control
* For each new task, a feature branch should be checked out from the development branch.
* The new branch name should be based off the task e.g. task is check correct email input, branch name could be check-email-input.
* Pull requests require at least two approvals before merge.
* Click [here](https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet) for a Git command cheat sheet

## Comments
For comments, we subscribe to the idea that if the code should be explanatory. If it needs comments, then it is poorly thought out either in terms of naming or the code itself being overly complicated so it cannot be easily understood.

Commented out code should never be allowed be part of the code. If it's commented out; it should not be there.

## Classes and Functions
### Classes
Try to maintain small classes, ensuring that they have one responsibility rather than creating a "God class".

### Functions
Functions should be short and have a singular purpose. We strive to make sure that:
> **Functions should do one thing. They should do it well. They should do it only.**
> Robert C Martin - Clean Code

Avoid excessive number of arguments in your functions. Try to ensure there are no side effects.
Follow the 'don't repeat yourself' principle (DRY). Duplication bloats code and is inefficient.

## Testing
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

### References
Title | Author | Link
------------ | ------------- | -------------
Clean Code | Robert C Martin | [Authors Website](http://cleancoder.com/products)
7 key coding practices for agile developers | Isaac Sacolick | [Article Link](https://www.infoworldcom/article/3446439/7-key-coding-practices-for-agile-developers.html)
How to write clean code? | Shubham Gupta |[Article Link](https://medium.com/mindorks/how-to-write-clean-code-lessons-learnt-from-the-clean-code-robert-c-martin-9ffc7aef870c)
Coding Standards and Conventions in Software Development Teams| Prince Sengayire |[Article Link]( https://medium.com/@psengayire/the-importance-of-coding-standards-and-conventions-in-the-software-development-team-how-they-can-5d252556a05#:~:text=Coding%20standards%20are%20collections%20of,methods%20for%20a%20programming%20language.&text=Without%20the%20coding%20conventions%2C%20every,code%20in%20the%20near%20future.)
ARRANGE-ACT-ASSERT: A PATTERN FOR WRITING GOOD TESTS | Automation Panda | [Article link](https://automationpanda.com/2020/07/07/arrange-act-assert-a-pattern-for-writing-good-tests/)
Gitflow Workflow | Atlassian | [Tutorial Link](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow#:~:text=The%20overall%20flow%20of%20Gitflow,branch%20is%20created%20from%20master&text=When%20the%20release%20branch%20is,to%20both%20develop%20and%20master)
Code Formatting Guide | Nick Schäferhoff | [Article Link](https://torquemag.io/2019/07/code-formatting-guide/)
Java Style Guide | Google | [Article Link](https://google.github.io/styleguide/javaguide.html#s4-formatting)
Code Formatting Patterns | Cunningham & Cunningham, Inc. | [Article Link](http://c2.com/ppr/formatting.html#6)
Naming Conventions | Wikipedia | [Article Link](https://en.wikipedia.org/wiki/Naming_convention_(programming)#:~:text=In%20computer%20programming%2C%20a%20naming,in%20source%20code%20and%20documentation)



