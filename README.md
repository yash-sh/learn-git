# learn-git

## Download and Install Git
> ### Windows
> + Download setup from here [32bit](https://github.com/git-for-windows/git/releases/download/v2.17.1.windows.2/Git-2.17.1.2-32-bit.exe) | [64bit](https://github.com/git-for-windows/git/releases/download/v2.17.1.windows.2/Git-2.17.1.2-64-bit.exe) and install it.
> + After installation run `setx GB "%PROGRAMFILES%\Git\bin\sh.exe"` (`%PROGRAMFILES%\Git` is the path where Git is installed by default) in your Command Prompt to use Git Bash easily from Command Prompt.

> ### Linux
> + For Debian/Ubuntu run `apt-get install git` in your terminal.
> + For others see command [here](https://git-scm.com/download/linux).

> ### Mac OSX
> + Download setup from [here](https://sourceforge.net/projects/git-osx-installer/files/git-2.17.1-intel-universal-mavericks.dmg/download?use_mirror=autoselect) and install it.

## Git Commands
+ help: `git help`
+ configure username: `git config --global user.name "username"`
+ configure email: `git config --global user.email "email"`
+ show username:  `git cofig user.name`
+ show email:  `git cofig user.email`
+ list of settings: `git config --list`
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
+ adding remote link: `git remote add remotename link`
+ seeing remote link: `git remote -v`
+ changing remote link: `git remote set-url remotename newlink`
+ push: `git push -u remotename branch`
+ fetch or pull: `git fetch remotename` then rebase by `git rebase`
OR
+ pull: `git merge remotename/branch`

## Few commands for navigation
+ Current directory: Linux : `pwd` | Windows : `cd`
+ Move to directory(one step down): Linux : `cd ..` | Windows : `cd ..`
+ list of files in directory: Linux : `ls` | Windows : `dir` or `dir /b` for simple list
+ list hidden files: Linux : `ls -la` | Windows : `dir /a:h` or `dir /a:h /b` for simple list
+ Move to directory(one step up): Linux : `cd dir_name` | Windows : `cd dir_name`

## Calling Git Bash in Command Prompt (for Windows)
+ If you didn't run the command (`setx GB "%PROGRAMFILES%\Git\bin\sh.exe"`) given above after installation of Git then run it to save Git Bash path as environment variable.
+ After adding GB as environment variable for Git Bash path close the that Command Prompt and open new Command Prompt to save changes.
+ Now you can enter into Git Bash in same Command Prompt window using command `call "%GB%" --login` and can return to Command Prompt by using `exit`.

## Github from git
+ Create new repository on Github with no README.md, .gitignore and license. You can add them later.
+ You will get HTTPS and SSH link there and instructions to use them.
+ Now move to your project directory by `cd project_directory_path`.
+ For existing project
  - Create .gitignore file bye `echo "excluded_folder" >> .gitignore`
  - Add all files by `git add .`
  - Commit your changes by `git commit -m "Create .gitignore file and add all files"`
  - Add remote link by `git remote add origin HTTPS_or_SSH_link`
  - Push all files to remote by `git push -u origin master`
+ For new project
  - Initialise git by `git init`
  - Create README.md file by `echo "# Repository Name" >> README.md`
  - Add README.md file by `git add README.md` or add all files by `git add .`
  - Commit changes by `git commit -m "Create README.md file and add it"`
  - Add remote link by `git remote add origin HTTPS_or_SSH_link`
  - Push all files to remote by `git push -u origin master`
