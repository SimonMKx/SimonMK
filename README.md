 # SimonMK

g@g-2:~$ mkdir Testvaja
g@g-2:~$ cd Testvaja
g@g-2:~/Testvaja$ git init
Initialized empty Git repository in /home/g/Testvaja/.git/
g@g-2:~/Testvaja$ git add README.md
fatal: pathspec 'README.md' did not match any files
g@g-2:~/Testvaja$ git add Testvaja.md
fatal: pathspec 'Testvaja.md' did not match any files
g@g-2:~/Testvaja$ echo "# SimonMK" >> README.md
g@g-2:~/Testvaja$ git init
Reinitialized existing Git repository in /home/g/Testvaja/.git/
g@g-2:~/Testvaja$ git add README.md
g@g-2:~/Testvaja$ commit -m "first commit"
bash: commit: command not found
g@g-2:~/Testvaja$ git commit -m "first commit"

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

fatal: empty ident name (for <g@g-2.um.si>) not allowed
g@g-2:~/Testvaja$ ^C
g@g-2:~/Testvaja$ git config --global user.email "simon.malek@student.um.si"
g@g-2:~/Testvaja$ git config --global user.name "SimonMKx"
g@g-2:~/Testvaja$ ^C
g@g-2:~/Testvaja$ git commit -m "first commit"
[master (root-commit) e8a27d3] first commit
 1 file changed, 1 insertion(+)
 create mode 100644 README.md
g@g-2:~/Testvaja$ git remote add origin https://github.com/SimonMKx/SimonMK.git
g@g-2:~/Testvaja$ git push -u origin master
Username for 'https://github.com': SimonMKx
Password for 'https://SimonMKx@github.com': 
Counting objects: 3, done.
Writing objects: 100% (3/3), 225 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/SimonMKx/SimonMK.git
 * [new branch]      master -> master
Branch master set up to track remote branch master from origin.
g@g-2:~/Testvaja$ git push -u origin master

