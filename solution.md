Assignment 1.4 — Git Essentials I
This guide provides the step-by-step terminal commands, workflow practices, and commit examples to complete Assignment 1.4.

Step 1: Verify Git Installation
Open your terminal and check if Git is installed:

Bash
git --version
(If it returns a version number like git version 2.x.x, you're good to go. If not, download and install Git from git-scm.com.)

Step 2: Open Terminal in the Project Folder
Navigate to the project folder you created in the previous assignment:

Bash
cd web-development-practice
Step 3: Initialize the Git Repository
Convert the local folder into a tracked Git repository by running:

Bash
git init
Step 4: Configure Your Git Username and Email
Set up your global identity so your commits are attributed to you:

Bash
git config --global user.name "Your Full Name"
git config --global user.email "your.email@example.com"
Steps 5, 6 & 7: Make at Least 3 Meaningful Commits
Let's modify index.html step-by-step and create three distinct commits.

Commit 1: Add initial HTML boilerplate
Open index.html in VS Code and add basic HTML structure:

HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Web Dev Practice</title>
</head>
<body>
    <h1>Welcome to Web Development Practice</h1>
</body>
</html>
Run the tracking and commit commands:

Bash
git status
git add index.html
git commit -m "feat: add initial html boilerplate to index.html"
Commit 2: Add a navigation bar section
Update index.html to include a navigation menu:

HTML
<body>
    <nav>
        <a href="#">Home</a>
        <a href="#">About</a>
        <a href="#">Contact</a>
    </nav>
    <h1>Welcome to Web Development Practice</h1>
</body>
Check status and commit:

Bash
git status
git add .
git commit -m "feat: add navigation bar component"
Commit 3: Add a footer section
Update index.html to add a footer:

HTML
    <footer>
        <p>&copy; 2026 Web Development Practice</p>
    </footer>
</body>
</html>
Check status and commit:

Bash
git status
git add .
git commit -m "feat: add footer section and close html tags"
Verify Your Commit History
To view your three commits in a clean history format, run:

Bash
git log --oneline
You should see a list showing your three commit messages with their unique hashes.

Submission Record
Terminal Command Summary
Bash
git --version
cd web-development-practice
git init
git config --global user.name "Your Full Name"
git config --global user.email "your.email@example.com"

# After making changes for Commit 1
git add index.html
git commit -m "feat: add initial html boilerplate to index.html"

# After making changes for Commit 2
git add .
git commit -m "feat: add navigation bar component"

# After making changes for Commit 3
git add .
git commit -m "feat: add footer section and close html tags"

# View history
git log --oneline