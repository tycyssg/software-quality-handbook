
# Coding Standards

## Formatting

## Naming Conventions

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


