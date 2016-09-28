# GitCommands

####Here is a list of some basic Git commands to get you going with Git

### Create

- Create a new local repository
  - `git init`
- Clone an existing repository
  - `git clone [your_repository_url] `
  
### Track chages

- File status about local repository
  - `git status`
- Chages to remote[tracked] files
  - `git diff [source_branch] [target_branch]`

### Add file

- Add all changes in commit
  - `git add .`
- Add single file in commit
  - `git add -p [your_file_name]`

### Commit file

- Commit previously chaged file
  - `git commit`
- Commit all local changes
  - `git commit -a`
- Add single file in commit
  - `git add -p [your_file_name]`
- Amending the most recent commit message in editor
  - `git commit --amend`
- Amending the most recent commit message with new message
  - `git commit --amend -m "New commit message"`
 
### See history

- See all commit log details
  - `git log`
- See commit log details about single file
  - `git log -p [your_file_name]`
- Only the commits of a certain author
  - `git log --author=[author_name]`
- Compressed log in one line:
  - `git log --pretty=oneline`
- Log details only for changes files
  - `git log --name-status`

### Command for branch

- See all branch
  - `git branch -av`
- Switch exisiting branch
  - `git checkout [your_branch_name]`
- Create new local branch and switch to new branch
  - `git checkout -b [your_branch_name]`
- Delete a local branch
  - `git branch -d [your_branch_name]`
- Delete a remote branch
  - `git branch -dr [your_branch_name]`
- Add tag on current commit
  - `git tag [your_tag_name]`
  
### Remote

- See all remote repository url
  - `git remote -v`
- See info about remote repository
  - `git remote show [remote_repository_url]`
- Add remote repository 
  - `git remote add  [remote_repository_url]`
- Fetch all branch structure from remote
  - `git fetch`

### pull 

- Fetch all changes from remote directory
  - `git pull`
  - `git pull [remote] [branch]`

### push 

- Fetch all changes from remote directory
  - `git push`
  - `git push [remote] [branch]`
- Publish your tags
  - `git pull --tags`
  
### merge

- Merge branch into your current HEAD
  - `git merge [your_branch_name]`
- Solve conflics using mergetool
  - `git mergetool`

### rebase

- Rebase with HEAD branch
  - `git rebase [your_branch_name]`
- Continue rebase after resolving conflicts
  - `git rebase --continue`
- Abort rebase
  - `git rebase --abort`
  
### reset

- Discard all changes in your local branch
  - `git reset --hard HEAD`
- Discard local branch changes for single file
  - `git checkout HEAD [your_file_name]`
- Revert specific commit
  - `git revert [commit_hash]`
- Reset your local branch with specific commit forcefully and discard local changes
  - `git reset --hard [commit_hash]`
- Reset your local branch with specific commit and discard local changes
  - `git reset [commit_hash]`
  
- Use colorful git output
  - `git config color.ui true`
  

## References

- https://help.github.com/
- https://git-scm.com/doc
