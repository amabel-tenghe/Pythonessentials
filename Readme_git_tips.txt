#Initialise git in a local repo
git init

# Undo git init in a local repo
rm -rf .git

#Tell git to start tracking file or stage file
git add <file name> 

#Record or register changes of staged files to the repository
git commit -m "message"

#Show list of files currently being tracked under branch master
git ls-tree -r master --name-only

#List all files that ever existed (i.e., including deleted file)
git log  --pretty=format: --name-only --diff-filter=A | sort - | sed '/^&/d'

#Create a new branch
git checkout -b <my branch name>

