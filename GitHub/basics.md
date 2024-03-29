# Git

## Git and GitHub

-   Git can keep track of changes made to code, synchronize code between different people, test changes to code without losing the original, and revert back to old versions of code.
-   GitHub is a website that stores Git repositories on the internet to facilitate the collaboration that Git allows for. A repository is simply a place to keep track of code and all the changes to code.
-   Git commands:
    -   `git clone <url>` : take a repository stored on a server (like GitHub) and downloads it
    -   `git add <filename(s)>` : add files to the staging area to be included in the next commit
    -   `git commit -m "message"` : take a snapshot of the repository and save it with a message about the changes
    -   `git commit -am <filename(s)> "message"` : add files and commit changes all in one
    -   `git status` : print what is currently going on with the repository
    -   `git push` : push any local changes (commits) to a remote server
    -   `git pull` : pull any remote changes from a remote server to a local computer
    -   `git log` : print a history of all the commits that have been made
    -   `git reflog` : print a list of all the different references to commits
    -   `git reset --hard <commit>` : reset the repository to a given commit
    -   `git reset --hard origin/master` : reset the repository to its original state (e.g. the version cloned from GitHub)
-   When combining different versions of code, e.g. using `git pull`, a merge conflict can occur if the different versions have different data in the same location. Git will try to take care of merging automatically, but if two users edit, for example, the same line, a merge conflict will have to be manually resolved.
    -   To resolve a merge conflict, simply locally remove all lines and code that are not wanted and push the results.
