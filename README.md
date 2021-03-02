# exercise3

celozzid1@csc330-02:~/erik_exercise1$ cd ..
celozzid1@csc330-02:~$ mkdir exercise3
celozzid1@csc330-02:~$ cd exercise3
celozzid1@csc330-02:~/exercise3$ git init
Initialized empty Git repository in /home/celozzid1/exercise3/.git/
celozzid1@csc330-02:~/exercise3$ git remote add origin https://github.com/celozzid1/exercise3
celozzid1@csc330-02:~/exercise3$ micro main.py
celozzid1@csc330-02:~/exercise3$ git add main.py
celozzid1@csc330-02:~/exercise3$ git commit -m "production"
[master (root-commit) 0100ac0] production
 1 file changed, 1 insertion(+)
 create mode 100644 main.py
celozzid1@csc330-02:~/exercise3$ git branch feature1
celozzid1@csc330-02:~/exercise3$ git branch
  feature1
* master
celozzid1@csc330-02:~/exercise3$ git switch feature1
git: 'switch' is not a git command. See 'git --help'.
celozzid1@csc330-02:~/exercise3$ git --help
celozzid1@csc330-02:~/exercise3$ git checkout feature1
Switched to branch 'feature1'
celozzid1@csc330-02:~/exercise3$ git branch
* feature1
  master
celozzid1@csc330-02:~/exercise3$ micro main.py
celozzid1@csc330-02:~/exercise3$ git add main.py
celozzid1@csc330-02:~/exercise3$ git commit -m "added new feature"
[feature1 103cdb5] added new feature
 1 file changed, 1 insertion(+)
celozzid1@csc330-02:~/exercise3$ git checkout master
Switched to branch 'master'
celozzid1@csc330-02:~/exercise3$ micro main.py
celozzid1@csc330-02:~/exercise3$ git merge feature1
Updating 0100ac0..103cdb5
Fast-forward
 main.py | 1 +
 1 file changed, 1 insertion(+)
celozzid1@csc330-02:~/exercise3$ ;s
-bash: syntax error near unexpected token `;'
celozzid1@csc330-02:~/exercise3$ ls
main.py
celozzid1@csc330-02:~/exercise3$ micro main.py
celozzid1@csc330-02:~/exercise3$ git branch -d feature1
Deleted branch feature1 (was 103cdb5).
celozzid1@csc330-02:~/exercise3$ git push origin master
Username for 'https://github.com': celozzid1
Password for 'https://celozzid1@github.com': 
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 2 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (6/6), 477 bytes | 477.00 KiB/s, done.
Total 6 (delta 0), reused 0 (delta 0)
To https://github.com/celozzid1/exercise3
 * [new branch]      master -> master
celozzid1@csc330-02:~/exercise3$ 
