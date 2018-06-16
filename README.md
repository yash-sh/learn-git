# learn-git
+ configure username: `git config --global user.name "username"`
+ configure email: `git config --global user.email "email"`
+ show username:  `git cofig user.name`
+ show email:  `git cofig user.email`
+ list of settings: `git config --list`
+ help: `git help`
+ For Navigation
  - Current directory: Linux : `pwd` | Windows : `cd`
  - Move to directory(one step down): Linux : `cd ..` | Windows : `cd ..`
  - list of files in directory: Linux : `ls` | Windows : `dir` or `dir /b` for simple list
  - list hidden files: Linux : `ls -la` | Windows : `dir /a:h` or `dir /a:h /b` for simple list
  - Move to directory(one step up): Linux : `cd dir_name` | Windows : `cd dir_name`
+ Initialising Repository: `git init`
+ adding all changes:`git add .`
+ adding specific changes:`git add filename`
+ commit: `git commit -m "message"`
+ commits history: `git log`
+ commits from a specific person: `git log --author="name"`
+ status: `git status`
+ differences(before staging or adding):`git diff`
+ differences(after staging or adding):`git diff --staged`
+ delete: `git rm filename`
+ rename: `git mv oldname newname`
+ commiting directly to repo: `git commit -am "message"`
+ making repository as working copy:`git checkout --filename`
+ unstaging changes: `git reset HEAD filename`
+ changing to older version: `git checkout ID --filename`
+ making remote: `git remote add remotename link`
+ push: `git push -u remotename branch`
+ fetch or pull: `git fetch remotename` then rebase by `git rebase`
OR
+ pull: `git merge remotename/branch`
