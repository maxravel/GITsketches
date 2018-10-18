#GIT SKETCHES 

unsafe method of merging:  
git checkout master  
git pull origin master  
git merge test  
ESC ":wq"  
git push origin master  
  
Keep gh-pages up to date with a master branch  
$ git add .  
$ git status // to see what changes are going to be commited  
$ git commit -m 'Some descriptive commit message'  
$ git push origin master  
  
$ git checkout gh-pages // go to the gh-pages branch  
$ git rebase master // bring gh-pages up to date with master  
$ git push origin gh-pages // commit the changes  
$ git checkout master // return to the master branch  
  
Basics:  
git init
touch index.html  
git status  
git add index.html  
git rm --cached index.html  
git add .  
git commit -m "message about commit"  
git log   //showing history of commitments  
git log --oneline //showing only one line about each commitment  
checkout commit  
git checkout 'id of commit here'  // go back to commit  
revert commit  
git revert 'id of commit here' // revert changes of commit  
reset commit  
git reset 'id of commit here' // reset commitments after id  
git reset 'id of commit here' --hard  
q - quiet  
h - help  

Branch:  
git branch 'name of branch'  
git branch -a  //showing branches  
git branch -D 'name of branch' //delete branch  
git checkout -b 'name of branch' // creating new branch and checkout it  

Merge: (to master) 
git checkout master  
git merge 'name of branch which you want merge'  
git push -u origin master


Hello Roman Tutorial:  
(upradging workflow)  
git config --global core.editor nano //changing git editor from vim to nano  
git config --global core.editor vim  
git commit --amend - updating commit //after pushing commit witch you upradge after push => git push --force  

In vim, you can press "i" to start entering text and save by pressing "esc" and ":wq" and "enter", this will commit with the message you typed. In your current state, to just come out without committing, you can do :q instead of the :wq as mentioned above.

git reset --hard //deleting changes on branch after last commit  
git reflog //back to last good state  
git stash //something like commit but not commit - storage of version, when you don't want to commit  