REFER commands.txt file for each task used and outputs

# 4. Version Control using Git
- Tasks
    1. **Initialize, Commit, and Branch Basics**
        
        **Objective:**
        
        - Initialize a new Git repository.
        - Create a few files and commit them.
        - Create a new branch, make changes, and merge it back to the main branch.
        
        **Requirements:**
        
        - Use `git init`, `git add`, and `git commit` to start your repository.
        - Create a branch using `git branch` or `git checkout -b` and switch between branches.
        - Merge the branch back to the main branch and verify the commit history.
    2. **Using .gitignore and Tracking Files**
        
        **Objective:**
        
        - Set up a `.gitignore` file to exclude certain files or directories.
        - Verify that ignored files are not tracked by Git.
        
        **Requirements:**
        
        - Create a `.gitignore` file with patterns (e.g., ignoring log files or temporary files).
        - Add files that match and do not match the ignore patterns.
        - Use `git status` to confirm which files are being tracked.
    3. **Undoing Changes and Reverting Commits**
        
        **Objective:**
        
        - Experiment with undoing changes in your working directory and commits.
        
        **Requirements:**
        
        - Modify a tracked file and use `git checkout -- <file>` (or `git restore`) to undo changes.
        - Make a commit, then use `git revert` or `git reset` to see how you can undo a commit safely.
        - Explain the differences between these approaches.
    4. **Simulating and Resolving Merge Conflicts**
        
        **Objective:**
        
        - Create a scenario that produces a merge conflict and resolve it.
        
        **Requirements:**
        
        - Create two branches from the same commit.
        - Modify the same line(s) of code in a common file in both branches.
        - Attempt to merge the branches, observe the conflict, and resolve it manually.
        - Use `git status` and `git diff` to identify and resolve the conflicting changes.
    5. **Interactive Rebasing for Clean Commit History**
        
        **Objective:**
        
        - Use interactive rebase to tidy up your commit history.
        
        **Requirements:**
        
        - Create a series of commits (some with minor changes or typos in commit messages).
        - Run `git rebase -i HEAD~n` (with `n` representing the number of commits) to squash, reorder, and edit commit messages.
        - Explain how squashing helps in cleaning up commit history before merging into a main branch.
    6. **Stashing Changes for Context Switching**
        
        **Objective:**
        
        - Learn how to use Git stash to save uncommitted work temporarily.
        
        **Requirements:**
        
        - Make changes in your working directory without committing.
        - Use `git stash` to save these changes.
        - Switch branches, perform some work, then return and reapply your stashed changes with `git stash pop`.
        - Optionally, demonstrate how to view and manage multiple stashes using `git stash list` and `git stash drop`.
    7. **Cherry-Picking Commits Between Branches**
        
        **Objective:**
        
        - Selectively apply a commit from one branch to another using cherry-pick.
        
        **Requirements:**
        
        - Create two branches with distinct commits.
        - Identify a commit on one branch that you want to apply to the other.
        - Use `git cherry-pick <commit-hash>` to apply the commit and handle any conflicts if they arise.
        - Verify the commit history to ensure the cherry-picked commit is present.
    8. **Using Git Hooks for Automated Checks**
        
        **Objective:**
        
        - Set up a Git hook to run scripts (like linters or tests) before commits are finalized.
        
        **Requirements:**
        
        - Create a `pre-commit` hook in the `.git/hooks` directory.
        - Write a simple script (e.g., a shell script or Node script) that runs a linter or a unit test.
        - Ensure that if the tests or linting fail, the commit is aborted.
        - Document how Git hooks can improve code quality in collaborative projects.
    9. **Working with Remote Repositories and Collaboration**
        
        **Objective:**
        
        - Simulate a collaborative workflow with remote repositories.
        
        **Requirements:**
        
        - Create a local repository and push it to a remote service (e.g., GitHub or GitLab).
        - Create a feature branch, make commits, and push the branch to the remote.
        - Open a Pull Request (or Merge Request) and perform a code review process.
        - Merge the feature branch into the main branch on the remote and then pull the changes locally.
    10. **Comprehensive Workflow with Forced Pushes and RecoveryObjective:Requirements:**
        - Simulate an advanced Git scenario that includes forced pushes, recovering lost commits, and a multi-branch workflow.
        - Create a repository with multiple branches representing features, bug fixes, and releases.
        - Simulate a scenario where a forced push (`git push --force`) is required (for example, after rewriting history with an interactive rebase).
        - Use `git reflog` to locate and recover lost commits after a mistaken force push.
        - Document each step, explaining how and why forced pushes should be handled with care, and how `git reflog` can be a lifesaver.
        - Discuss best practices for collaborating with teams when rewriting history and using force pushes.