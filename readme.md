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

Branch:  
git branch 'name of branch'  
git branch -a  //showing branches  
git branch -D 'name of branch' //delete branch  
git checkout -b 'name of branch' // creating new branch and checkout it  

Merge:  
git checkout master  
git merge 'name of branch which you want merge'  

