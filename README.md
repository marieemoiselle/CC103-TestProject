# CC 103 - Test Project
*by: Ms. Fatima Marie P. Agdon, MSCS*

[![LinkedIn](https://custom-icon-badges.demolab.com/badge/LinkedIn-0A66C2?logo=linkedin-white&logoColor=fff)](https://www.linkedin.com/in/fatimamarieagdon/) 
[![GitHub](https://img.shields.io/badge/GitHub-%23121011.svg?logo=github&logoColor=white)](https://github.com/marieemoiselle)

This is a repository intended to be helpful for the Git and GitHub. This will walk you through setting up Git, creating your first project, connecting to GitHub, and collaborating with your team using proper Git workflows. Whether you're coding solo or working in a team, this guide will help you track your progress, manage your project efficiently, and avoid common pitfalls.  

---
## ✧˖°. ┆∿ Importance
Knowing Git and GitHub is important because they help you manage your code efficiently, track every change, and collaborate safely with others. For the long term:
- **History & Backup**. You can go back to any previous version of your project. No more lost work.
- **Collaboration**. Multiple people can work on the same project without overwriting each other's changes.
- **Professional Skill**. Git/GitHub are standard in the industry. Knowing them makes your work reproducible, organized, and easier to share.
- **Project Growth**. As projects get bigger, version control helps maintain structure, review code, and track progress over months or years.

## ✧˖°. ┆∿ Definition of Terms
1. 🧠 ***Git (The Brain).*** It is a version control system that tracks changes in your code. This contains the *history* of your project, where you can go back to previous versions of it. <br/>
2. ☁️ ***GitHub (The Cloud).*** It is a website where you store your Git projects online that is used for sharing & collaboration. This is like Google Drive, but for codes.<br/>
3. 📝 ***Repository (Repo).*** It is a storage space for your project. Can be local (on your computer) or remote (on GitHub).<br/>
4. 🌿 ***Branch.*** It is a separate line of development in a project. The *parallel universe* for your code.<br/>
5. 🔀 ***Merge.*** It is a process of combining changes from one branch into another (usually into main).<br/>
6. 🕵️ ***Pull Request (PR).*** It is a request to merge your changes into another branch. Team members can review before approving.<br/>
7. 📥 ***Clone.*** It is a process of making a copy of a repository on your local machine from GitHub.<br/>
8. ⬆️ ***Push.*** It is a process of sending your local commits to the remote repository on GitHub.<br/>
9. ⬇️ ***Pull.*** It is a process of getting the latest updates from a remote repository to your local machine.<br/>
10. 💾 ***Commit.*** It is a snapshot of your project at a specific point in time.<br/>
11. 🎭 ***Staging Area.*** It is a temporary space where Git holds changes before they are committed. This is the preparation of files for a snapshot.

---
## ✧˖°. ┆∿ First Time Setup (One-Time Only)

### Install Git
Download [Git](https://git-scm.com/install/windows) and install it.

### Check Installation
```bash
git --version
```

### Set Your Identity
```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

## ✧˖°. ┆∿ Creating Your First Project
1. Create a folder named Projects.
2. Right-click the folder → Open Git Bash here.
3. Create Project Folder
```bash
mkdir CC103-FinalProject-CS1207-Team1
cd CC103-FinalProject-Team1
```
*Note: Change the team number and section accordingly.*

`mkdir` → make directory
`cd` → change directory

### Initialize Git
```bash
git init
```

## ✧˖°. ┆∿ The Core Cycle

### Adding `.gitignore`
It is a key concept that prevents unnecessary or sensitive files from being tracked by Git. This is useful for files that *don’t need to be shared*, like:
- Compiled binaries (`.exe`, `.dll`)
- Temporary files (`.tmp`, `.log`)
- IDE or system-specific files (`.vscode/`, `Thumbs.db`)
Example:
```
# Ignore all .exe files
*.exe
# Ignore VS Code folder
.vscode/
```
**How to add .gitignore**
1. Create a new text file
2. Name it as .gitignore
   
💡 **TIP:** Always create a `.gitignore` before committing your project to avoid cluttering the repository with unnecessary files.

### Add Files
```bash
git add .
```
This tells Git to track the changes you made.

### Commit Changes
```bash
git commit -m "Initial Commit"
```
This saves your current version.
*REMEMBER: Commit messages should be specific and meaningful.*
Examples:
`Changes in the delete function`
`FIX: add function now handles invalid input`

### Connecting to GitHub
1. Sign in to GitHub
2. Create a repository. Set your repository name (include your team number and section)
3. Link Local Project to GitHub
```bash
git remote add origin https://github.com/username/your-repo.git
```
*REMEMBER: Do NOT copy-paste the example link. Use your own repository link.*

### Upload Your Code
```bash
git push -u origin main
```
### Standard Workflow
```bash
git add .
git commit -m "Describe what you changed"
git push
```
- `git add` Adds changes to the **staging area**. Only changes added here will be included in the next commit.  
- `git commit` Saves the staged changes to your repository as a snapshot with a message describing what changed. Note: Commit messages are mandatory
---

## ✧˖°. ┆∿ Collaboration
The team leader will:
- Create the repository
- Invite members as collaborators
### Steps (Leader Only)
1. Go to repository → Settings
2. Select Collaborators under Access
3. Authenticate if required
4. Click Manage Access → Add People
5. Search and add teammates

*Note: Invitations expire after 7 days.*

## ✧˖°. ┆∿ For Team Members (After Accepting Invitation)
### Clone the Repository
```bash
git clone https://github.com/username/project.git
cd project
```
### Get Latest Updates
```bash
git pull
```
### Create a Branch
```bash
git checkout -b test-branch
```
### Work and Save Changes
```bash
git add .
git commit -m "Describe what you changed"
git push origin test-branch
```
### Next Step
Create a Pull Request to merge your changes into the main branch.

---

## ✧˖°. ┆∿ Quick Reference Commands
| Command                       | Purpose                     |
| ----------------------------- | --------------------------- |
| `git init`                    | Initialize a Git repository |
| `git add .`                   | Track all changes           |
| `git commit -m "msg"`         | Save snapshot with message  |
| `git remote add origin <url>` | Link local repo to GitHub   |
| `git push`                    | Upload commits to GitHub    |
| `git pull`                    | Get latest updates          |
| `git checkout -b <branch>`    | Create new branch           |

---

## ✧˖°. ┆∿ Test Activity
1. Clone the repository
2. Make changes
3. Submit a pull request
