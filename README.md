# Git and GitHub Project Structure and Workflow with Branches and Merging.

## initialize repository (not needed if it's already on GitHub)
git init

## replicates a remote repository (run this if it's on GitHub)
git clone https://github.com/TechLabs-Berlin/wt21-schedule-n 

## changes directory
cd wt21-schedule-n/

## lists all remote branches (optional)
git branch -r

## changes to existing branch
### List of branches: https://github.com/TechLabs-Berlin/wt21-schedule-n/branches
git checkout suliyat

## lists local branches (optional)
git branch

## gets latest changes
git pull

## see status of local git repository
git status

## marks a change for commit
git add .

## commits all added changes
git commit -m "Changed README.md"

## sends all commits to remote repository (on GitHub)
git push

## creates and moves to local branch "emmanuel"
git checkout -b "emmanuel"

## pushes local branch to remote branch
git push --set-upstream origin emmanuel

## gets latest list of branches (use it if someone pushed a new branch to GitHub)
git fetch

## gets changes from another branch to my branch
git pull origin suliyat

### if git asks to specify how to reconcile branches
git pull origin suliyat --rebase
git rebase --continue

## delete branch (careful)
git branch -d name_of_branch