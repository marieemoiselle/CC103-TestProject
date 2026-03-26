# CC 103 - Test Project
*by: Ms. Fatima Marie P. Agdon, MSCS*

[![LinkedIn](https://custom-icon-badges.demolab.com/badge/LinkedIn-0A66C2?logo=linkedin-white&logoColor=fff)](https://www.linkedin.com/in/fatimamarieagdon/) 
[![GitHub](https://img.shields.io/badge/GitHub-%23121011.svg?logo=github&logoColor=white)](https://github.com/marieemoiselle)
---

## ✧˖°. ┆∿ Definition of Terms
🧠 **Git (The Brain).** A version control system that tracks changes in your code. This contains the “history” of your project, where you can go back to previous versions of it. <br/>
☁️ **GitHub (The Cloud).** A website where you store your Git projects online that is used for sharing & collaboration. This is like Google Drive, but for codes.

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
---

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
---

## ✧˖°. ┆∿ The Core Cycle
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
