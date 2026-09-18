\# Git Team Sync Workflow



\## 1. Rejected Push Error



The rejected push showed the error `(fetch first)` and said that the remote contained work that I did not have locally. This happened because another clone had already pushed changes to the same feature branch, so my local branch was behind the remote branch. Git rejected the push because it could not safely perform a fast-forward update.



\## 2. Merge vs. Rebase



In Task 3, I used merge to combine the changes from the two clones. This preserved both lines of development and created a merge commit that connected the two histories.



In Task 4, I used rebase instead. Rebase took my local commit and replayed it on top of the updated remote branch, producing a more linear history. Unlike merge, rebase changes the commit history and creates a new commit ID.



\## 3. Habit That Could Prevent Rejected Pushes



A useful habit is to fetch or pull the latest changes from the remote branch before starting work or pushing changes. This helps make sure my local branch is synchronized with the team's latest work.



\## 4. Merge or Rebase on a Shared Team Branch



I would generally use merge on a shared team branch because it preserves the existing shared history and does not rewrite commits that other team members may already have. Rebase can be useful for organizing work before it is shared, but extra care is needed when rebasing commits that are already part of a shared branch.

