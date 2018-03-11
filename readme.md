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