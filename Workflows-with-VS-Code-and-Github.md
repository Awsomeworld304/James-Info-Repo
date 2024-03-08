# Workflows with VS Code and Github
- [Workflows with VS Code and Github](#workflows-with-vs-code-and-github)
  - [Git](#git)
    - [Explanation](#explanation)
    - [Terminology](#terminology)
    - [Best Practices](#best-practices)
      - [Dos and Don'ts](#dos-and-donts)
      - [Branching Strategy](#branching-strategy)
  - [GitHub](#github)
    - [Making Pull Requests](#making-pull-requests)
      - [Website](#website)
      - [VS Code](#vs-code)
  - [VS Code + Extensions](#vs-code--extensions)
  - [Misc.](#misc)
    - [Commit Messages](#commit-messages)
## Git
### Explanation
Git is a version control software.\
Paired with GitHub, gives you a lot of tools as a programmer.\
Pull Requests, Pushing, Checking Out, Forking and more.\
Never used git? Don't worry, it's not that hard, as the extra tools installed will add GUI elements.
### Terminology
Commit - Commit your code to be pushed.\
Stage - Stage your code for the next commit.\
Push - Push modified code to the origin branch.\
Pull - Pull modified code from origin branch.\
Sync - Sync the origin and local branch.\
Checkout* - Switch to a different branch.\
Rebase* - Change the base of your commit to another.\
*You normally won't have to use this, but if you do, get confirmation from another to prevent human error if you're unsure!
### Best Practices
#### Dos and Don'ts
- Do: Make a pull request when ready to merge.
  - Don't: Auto merge the pull request without any review especially if it's a big modification.
- Do: Stage and commit your changes.
  - Don't: Send the commit with a stupid message. Make it concise and quick.
  - Don't Upload the code through the website.
  - [Commit Messages](#commit-messages)
- Do: Write clean neat code.
  - Don't: Write messy or obfuscated code that is hard to read and understand.
- Do: Add comments. They are very useful.
  - Don't: Add stupid comments. I know how tempting it is, but if it's not useful then don't write it.
<!-- -->
#### Branching Strategy
Your workflow to branching.\
There are different types including:
- Centralized workflow: Teams use only a single repository and commit directly to the main branch.
- Feature branching: Teams use a new branch for each feature and don't commit directly to the main branch.
- GitFlow: An extreme version of feature branching in which development occurs on the develop branch, moves to a release branch, and merges into the main branch.
- Personal branching: Similar to feature branching, but rather than develop on a branch per feature, it's per developer. Every user merges to the main branch when they complete their work.
<!-- -->
The best method of branching is (atomic) feature branching.\
Atomic as in one feature, bug fix, or patch per branch.\
This makes it easier to review code for merging and prevents unintentional messes.
## GitHub
This will discuss how to do various actions on GitHub.
### Making Pull Requests
This depends on your method.\
You cannot do it from the terminal as it is a GitHub feature, not one from git itself.
I do not recommend doing this through the desktop app.
#### Website
Start from your repo, and click the 'Pull Requests' tab at the top.\
(img)\
Press ```New pull request```.\
(img)\
In the ```compare:``` tab, select your branch that you want to merge.\
(img)\
Review your code to make sure that it's good, and that the title is concise along with the description.\
Once you're ready, press ```Create pull request```.
If you need to require approval, then invite a reviewer to look at it and approve it.\
If everything looks good then press the ```Merge pull request``` button.\
From here you can press the ```Confirm merge``` button to finalize the merge.\
You can delete the branch, which in most cases is preferred as seen in [Feature branching](#branching-strategy).
#### VS Code
This is easier than on the website.
wip
## VS Code + Extensions
wip
## Misc.
Misc. info or more in-detail explanations.
### Commit Messages
Describe your changes in imperative mood, e.g. “make x do y” instead of “[This patch] makes x do y” or “[I] changed x to do y,” as if you are giving orders to the codebase to change its behavior. Try to make sure your explanation can be understood without external resources. Instead of giving a URL to a mailing list archive, summarize the relevant points of the discussion.
