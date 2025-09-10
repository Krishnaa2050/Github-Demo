## The GitHub Workflow: A Step-by-Step Guide

### Step 1: Fork the Repository

The first step is to create your own personal copy, or **fork**, of the project on GitHub. This gives you a safe space to make changes without affecting the original project. To do this, simply click the **Fork** button in the top-right corner of the repository's page on GitHub. This creates an exact copy of the project under your own GitHub account.

### Step 2: Clone the Repository to Your Computer

Now that you have your own copy, you need to download it to your local machine. This is called **cloning**. Go to your newly forked repository's page, click the green **Code** button, and copy the HTTPS URL.

Then, open your terminal (or command prompt on Windows) and run the following command:

```bash
git clone [paste the URL here]
```

This command downloads all the project's files and the complete Git history to your computer.

### Step 3: Create a New Branch

Before you make any changes, you should create a new **branch**. A branch is like a separate, isolated timeline for your work. It lets you develop new features or fix bugs without disturbing the main project. Think of the `main` branch as the official, stable version of the project.

To create a new branch, use the following command:

```bash
git checkout -b your-branch-name
```

For example, `git checkout -b add-my-info`. This command creates and switches you to the new branch in one step.

### Step 4: Make and Commit Your Changes

Now you're ready to make your changes\! Open the `contributors.md` file in a text editor and add your name.

Once you've saved the file, you need to tell Git that you're ready to save these changes. This two-part process is called **committing**.

First, you **stage** your changes with the `git add` command. This tells Git which files you want to include in your next save.

```bash
git add contributors.md
```

Then, you **commit** the staged changes with a descriptive message. This creates a "snapshot" of your work at this point in time.

```bash
git commit -m "Add your-name to contributors list"
```

A good commit message explains what you changed and why. It's like a note to yourself and your collaborators.

### Step 5: Push Your Branch to GitHub

Now your changes are saved locally on your computer. To upload them to your personal repository on GitHub, you need to **push** them.

```bash
git push origin your-branch-name
```

This command uploads your new branch and all its commits to your remote repository on GitHub. The `origin` keyword is a shortcut for the URL of your repository.

### Step 6: Create a Pull Request

This is the final step where you propose your changes to the original project. Go to your forked repository's page on GitHub. You should see a yellow banner asking if you'd like to create a **pull request** (PR) for your newly pushed branch.

A pull request is a formal request to "pull" your changes into the main project. It's a key part of the collaboration process because it allows the project maintainers to review your code and discuss it with you before it's merged.

Once your pull request is approved and merged, your changes will officially become part of the main project.

-----

### Basic Commands Reference

| Command | Purpose |
| :--- | :--- |
| `git clone [URL]` | Downloads a repository to your computer. |
| `git status` | Shows which files have been changed. |
| `git branch` | Lists all local branches. |
| `git checkout [branch-name]` | Switches to a different branch. |
| `git add [file-name]` | Stages a file for the next commit. |
| `git commit -m "[message]"` | Saves the staged changes with a message. |
| `git push` | Uploads your local commits to the remote repository. |
| `git pull` | Downloads and integrates changes from the remote repository. |
