PS D:\> mkdir git_exercises


    Directory: D:\


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----         8/31/2023  10:08 PM                git_exercises


PS D:\> cd git_exercises
PS D:\git_exercises> git status
fatal: not a git repository (or any of the parent directories): .git
PS D:\git_exercises> git init
Initialized empty Git repository in D:/git_exercises/.git/
PS D:\git_exercises> echo 'Hello World' > hello.txt
PS D:\git_exercises> git add hello.txt
PS D:\git_exercises> git commit -m "Initial commit"
[master (root-commit) 9c5496b] Initial commit
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 hello.txt
PS D:\git_exercises> tree .git
Folder PATH listing for volume New Volume
Volume serial number is 00A7-8D80
D:\GIT_EXERCISES\.GIT
├───fsmonitor--daemon
│   └───cookies
├───hooks
├───info
├───logs
│   └───refs
│       └───heads
├───objects
│   ├───9c
│   ├───bc
│   ├───f7
│   ├───info
│   └───pack
└───refs
    ├───heads
    └───tags
PS D:\git_exercises> cat .git/HEAD
ref: refs/heads/master
PS D:\git_exercises> cat .git/refs/heads/master
9c5496b007aa149542c69c2e3bbc37976f426819
PS D:\git_exercises> git log --oneline
9c5496b (HEAD -> master) Initial commit
PS D:\git_exercises> git branch Hanh_branch
PS D:\git_exercises> tree .git/refs
Folder PATH listing for volume New Volume
Volume serial number is 00A7-8D80
D:\GIT_EXERCISES\.GIT\REFS
├───heads
└───tags
