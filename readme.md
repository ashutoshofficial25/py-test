# Basic git commands

This repo includes git basic commands -

## Init a repo

## Add and push code & changes on github

## Check logs

## Working with stash .

Question : Steps 1

mkdir python-project
cd python-project

git init

touch app.py

print("Hello, Git!")

git status

git add .

git commit -m "Initial commit with app.py"

git remote add origin https://github.com/ashutoshofficial25/py-test.git

git remote -v

git branch -M main
git push -u origin main

Question 2 --

-- made changes in app.py file

print("Hello, Git!")
print("New Feature Added")

git status

git diff

git add -p app.py

git commit -m "Added new feature logic"

Question 3 --

git branch feature-update

git checkout feature-update

- make change in app.py
  def greet():
  print("Feature branch update")

greet()

git add app.py
git commit -m "Added greeting feature"

git checkout main

git merge feature-update

git log --oneline

git branch -d feature-update

git branch dummy-branch
git branch -D dummy-branch

Question 4 --

print("Temporary work")

git stash -u

git stash list

git stash apply

git add .
git commit -m "Restored stashed work"

print("Incorrect logic")

git add .
git commit -m "Added incorrect code"

git reset --soft HEAD~1

git add .
git commit -m "Added corrected logic"

git revert HEAD

git log --oneline
