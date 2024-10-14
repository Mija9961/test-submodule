# To add submodule
From the repo where you want to add execute the following commands:

git submodule add https://github.com/Mija9961/dmf.git cms/dmf

git submodule update --init --recursive

git add .

git commit -m "Readme.md changed"

git push origin main

# Push submodule changes
1. Push from the submodule

   git add .

   git commit -m "changes in submodule eao"

   git push

2. Push from main

   git add submodule_folder/submodule

   git commit -m "EAO:changes in submodule"

   git push origin main

# Merge feature branch to develop

git checkout develop

git merge feature/branch_name

Example: git merge feature/eao

git push origin develop

# Delete feature branch

git branch -d feature-branch-name  

git push origin --delete feature-branch-name

# Hotfix branch

A hotfix branch needs to be merged to both main and develop branch

1. git checkout main

   git merge hotfix/fix1

    git push origin main

2. git checkout develop

   git merge hotfix/fix1

    git push origin develop

3. Delete hotfix branch

   git branch -d feature-branch-name  

   git push origin --delete feature-branch-name