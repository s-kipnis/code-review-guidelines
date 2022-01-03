# code-review-guidelines

### Voting 
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

