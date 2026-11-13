Git is a distributed version control system used to track changes in source code during software development. Below is a categorized quick-reference guide to the most essential Git commands.

⚙️ Setup & Configuration

Before starting, set up your identifying details and initialize projects.
• Set username: git config --global user.name "Your Name"

• Set email: git config --global user.email "your.email@example.com"

• Initialize a new local repository: git init

• Clone an existing repository: git clone <url>



🔄 The Core Workflow (Stage & Commit)

This is the daily cycle used to save progress in your local environment.
• Check repository status: git status (shows modified, staged, or untracked files)

• Stage a specific file: git add <file>

• Stage all files: git add .

• View file modifications: git diff (shows unstaged changes)

• Commit staged changes: git commit -m "Your commit message"

• Modify the last commit: git commit --amend (fixes typos or forgotten files)



🌿 Branching & Merging

Isolate features or experiments without breaking the main codebase.
• List all local branches: git branch

• Create a new branch: git branch <branch-name>

• Switch to a branch: git switch <branch-name> (or git checkout <branch-name>)

• Create and switch to a branch instantly: git checkout -b <branch-name>

• Merge a branch into your active branch: git merge <branch-name>

• Safely delete a branch: git branch -d <branch-name>


☁️ Remote Syncing

Share your local progress or retrieve changes from a platform like GitHub or GitLab.

• Link local repo to a remote server: git remote add origin <url>

• View connected remote URLs: git remote -v

• Download remote changes without merging: git fetch

• Download remote changes and merge them: git pull

• Upload local commits to the server: git push origin <branch-name>



📜 Inspection & History

Review your project's timeline to understand what changed.

• View commit history: git log

• View a simplified, one-line history: git log --oneline

• See details of a specific commit: git show <commit-hash>

• Track who modified lines in a file: git blame <file>

🛠️ Undo & Discarding Changes

Safely remove mistakes or temporarily set aside incomplete work.
• Discard unstaged changes in a file: git restore <file>
• Unstage a file but keep its modifications: git reset <file>
• Hard reset to a specific commit (destroys changes): git reset --hard <commit-hash>
• Save uncommitted work temporarily: git stash
• Retrieve and apply your stashed work: git stash pop
