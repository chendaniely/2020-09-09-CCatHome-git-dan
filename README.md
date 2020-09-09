# 2020-09-09: CarpentryCon@Home git workshop

Etherpad: https://pad.carpentries.org/cchome-maintainer-git-skills

This was the second time I taught this workshop,
the video for the first time can be found here:
https://www.youtube.com/watch?v=uvWhSYBkZJ0

Carpentry Con at Home Git workshop Part 2

- git clone <url>: download the repo from the web to your computer
  - make sure you are not in another repo
  - just like git init do only one per repo

## Branches

- `git branch <branch_name>`: create a new branch where you are (`HEAD`)
- `git switch <branch_name>`: moves you to `<branch_name>`
  - `git checkout <branch_name>`: pre aug 2019 way to move to another branch

- shortcuts for creating branches, will create and move to them in 1 go:
    - `git checkout -b <branch_name>
    - `git switch -c <branch_name>

- `git branch -d <branch_name>`: this will delete <branch_name> on your local computer
- `git fetch --prune`: will update your local git tree with the remote
    - the prune will also delete references to branches that were deleted on the remote

- Each pull request is independent from one another
  - You won't know a merge conflict will happen until one of the PRs gets merged

- `git rebase <branch>`: rebases your current branch against `<branch>`, where `<branch>` is usually `master` or `gh-pages`
  - make sure you are already on the conflicting branch

## Additional resources

## Some additional notes and links

- Software Carpentry notes on basic git: https://swcarpentry.github.io/git-novice/
    - The setting up git has the commands to setup your name/email/editor: https://swcarpentry.github.io/git-novice/02-setup/index.html

- Git workflow notes and commands (to paste on your wall)
    - https://chendaniely.github.io/training_ds_r/help-faq.html

- Atlassian page on git workflows: https://www.atlassian.com/git/tutorials/comparing-workflows
    - The one we covered today was mainly the "Feature Branch Workflow": https://www.atlassian.com/git/tutorials/comparing-workflows/feature-branch-workflow

- The atlassian page has more infor about "git flow", but this is also another top Google hit that I liked:
  - https://nvie.com/posts/a-successful-git-branching-model/

- Getting your (bash) terminal to show current path and other things:
    - Use this to create your PS1 variable: http://bashrcgenerator.com/

- Show git branch in terminal:
    - In addition you can write a function and put that in your PS1 to also show git branch
    - https://gist.github.com/joseluisq/1e96c54fa4e1e5647940

- https://chendaniely.github.io/training_ds_r/help-faq.html (has the checklist)
- https://happygitwithr.com/ (more rstudio specific workflows)
- https://swcarpentry.github.io/git-novice/
- https://www.youtube.com/watch?v=uvWhSYBkZJ0
- Setting up ssh links: https://bi-sdal.github.io/training/ssh-keys.html
