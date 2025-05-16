DevOps Task-4 – Version-Controlled Workflow

=================================================

Objective:

Manage a DevOps project using Git best practices such as:
- Creating and using branches (main, dev, feature/*)
- Using Pull Requests (PRs)
- Adding a .gitignore file
- Tagging releases
- Documenting tasks using markdown
  
Tools Used:
-----------
- Git
- GitHub
- Terminal or Git Bash
------------------------------------------------------------
Step-by-Step Instructions
------------------------------------------------------------

1. Initialize Git Repository
Open terminal and run:
    mkdir Devops task project
    cd Devops task project
    git init

2. Create .gitignore File
Create the file:
    touch .gitignore
3. Create README File:
    touch README.txt
Add basic project info:
    DevOps Git Project
    This project follows Git best practices with branching, PRs, and versioning.
4. Make Initial Commit
    git add .
    git commit -m "Initial commit with README and .gitignore"
5. Create GitHub Repository and Push Code
- Go to https://github.com
- Create new repo: devops-project
- DO NOT add README or .gitignore on GitHub
Connect your local repo to GitHub:
    git remote add origin https://github.com/arjumandshafi/devops-task4
    git branch -M main
    git push -u origin main
6. Create and Push dev and feature Branches:
    git checkout -b dev
    git push -u origin dev
    git checkout -b feature
    git push -u origin feature
7. Work on the Feature Branch
Add new feature:
    Cat >> README.md
Inside README file modify some changes
    git add README.md
    git commit -m "modify"
    git push
8. Create Pull Request (PR) from feature/login to dev
- Go to GitHub
- Click "Compare & Pull Request"
- Base: dev, Compare: feature
- Add title and description
- Click "Create Pull Request"
- Click "Merge Pull Request"

9. Merge dev into main
- Go to GitHub
- Create PR from dev to main
- Review and merge the PR
10. Add a Version Tag (v1.0)
    git checkout main
    git pull
    git tag v1.0
    git push origin v1.0



