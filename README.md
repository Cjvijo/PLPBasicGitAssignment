# PLPBasicGitAssignment
//Navigating to dirve D in my local machine
- jonni@PULLMANHOTEL MINGW64 /
- $ cd d:

//Creating a Folder
- jonni@PULLMANHOTEL MINGW64 /d
- $ mkdir PLPBasicGitAssignment

//Navigating to created folder
- jonni@PULLMANHOTEL MINGW64 /d
- $ cd PLPBasicGitAssignment/

//Initializing git repository
- jonni@PULLMANHOTEL MINGW64 /d/PLPBasicGitAssignment
- $ git init
- Initialized empty Git repository in D:/PLPBasicGitAssignment/.git/

//Linking local repository to the GitHub repository created
- jonni@PULLMANHOTEL MINGW64 /d/PLPBasicGitAssignment (master)
- $ git remote add origin https://github.com/Cjvijo/PLPBasicGitAssignment.git

//Creating a text file using vim 
- jonni@PULLMANHOTEL MINGW64 /d/PLPBasicGitAssignment (master)
- $ vi hello.txt

//commands inside vim
- press i to insert simple text message "Hello,Git!"
- Press Esc :wq to write and quit vim

//Stage changes in my working directory for the next commit
- jonni@PULLMANHOTEL MINGW64 /d/PLPBasicGitAssignment (master)
- $ git add hello.txt
- warning: in the working copy of 'hello.txt', LF will be replaced by CRLF the next time Git touches it

//Error encountered for forgettin the "ls" command
- jonni@PULLMANHOTEL MINGW64 /d/PLPBasicGitAssignment (master)
- $ git --list
- unknown option: --list
- usage: git [-v | --version] [-h | --help] [-C <path>] [-c <name>=<value>]
             [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
             [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
             [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
             [--config-env=<name>=<envvar>] <command> [<args>]

//Correct command to list files and directories in the current directory
- jonni@PULLMANHOTEL MINGW64 /d/PLPBasicGitAssignment (master)
- $ ls
- hello.txt

//Record changes to th repository
- jonni@PULLMANHOTEL MINGW64 /d/PLPBasicGitAssignment (master)
- $ git commit -m "Add hello.txt with a greeting"
- [master (root-commit) c778d39] Add hello.txt with a greeting
 - 1 file changed, 1 insertion(+)
 - create mode 100644 hello.txt

//Upload to GitHub repository error
- jonni@PULLMANHOTEL MINGW64 /d/PLPBasicGitAssignment (master)
- $ git push -u origin main
- error: src refspec main does not match any
- error: failed to push some refs to 'https://github.com/Cjvijo/PLPBasicGitAssignment.git'

//Upload to GitHub repository using branch master
- jonni@PULLMANHOTEL MINGW64 /d/PLPBasicGitAssignment (master)
- $ git push -u origin master
- Enumerating objects: 3, done.
- Counting objects: 100% (3/3), done.
- Writing objects: 100% (3/3), 236 bytes | 236.00 KiB/s, done.
- Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
- remote:
- remote: Create a pull request for 'master' on GitHub by visiting:
- remote:      https://github.com/Cjvijo/PLPBasicGitAssignment/pull/new/master
- remote:
- To https://github.com/Cjvijo/PLPBasicGitAssignment.git
-  * [new branch]      master -> master
- branch 'master' set up to track 'origin/master'.
