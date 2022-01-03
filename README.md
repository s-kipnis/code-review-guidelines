# code-review-guidelines

## Targets of Code Review

- speeding up development
- improving knowledge distribution
- making better use of domain experts
- removing friction

## Should not be targets of Code Review

- design review. Design must be determined before coding.
- error finding. Most of errors should be finded using tests: unit, component and integration.

## When CL should be approved

Based https://google.github.io/eng-practices/review/reviewer/standard.html

### In general, reviewers should favor approving a CL once it is in a state where it definitely improves the overall code health of the system being worked on, even if the CL isn’t perfect.

*That is the senior principle among all of the code review guidelines.*

## Generic checklist

Based on https://google.github.io/eng-practices/review/

Important

- Functionality: Does the code behave as the author likely intended?
- **Tests: Does the code have correct and well-designed automated tests?**
- Naming: Did the developer choose clear names for variables, classes, methods, etc.?
- Side effects: Any unwanted or unexpected side effects? Critical for us.

Standard

- Design: Is the **code** well-designed?
- Complexity: Could the code be made simpler?
- Comments: Are the comments clear and useful?

Optional
- Style: Does the code follow our style guides? Usually should be done automatically.
- Documentation: Did the developer also update relevant documentation? Should be part of task.


## Voting 
Based on https://gerrit-review.googlesource.com/Documentation/config-labels.html

**-2 This shall not be merged**

The code is so horribly **incorrect/buggy/broken** that it must not be submitted to this project, or to this branch.
*Any -2 blocks submit.*

**-1 I would prefer this is not merged as is**

The code **doesn’t look right, or could be done differently**, but the reviewer is willing to live with it as-is if another reviewer accepts it.
*Does not block submit.*

**0 No score**

Didn’t try to perform the code review task, or glanced over it but don’t have an informed opinion yet.

**+1 Looks good to me, but someone else must approve**

The code looks right to this reviewer, but the reviewer doesn’t have access to the +2 value for this category.

**+2 Looks good to me, approved**

Basically the same as +1, but for those who have final say over how the project will develop.
*Any +2 enables submit.*

