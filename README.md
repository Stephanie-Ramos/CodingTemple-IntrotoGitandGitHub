# Introduction to Git and GitHub

## Project Description
This project introduces the fundamentals of Git and GitHub as tools for version control and collaborative workflows. It focuses on understanding how to track changes in files, manage project versions, and connect local repositories to remote repositories on GitHub. Through hands-on practice, the project demonstrates essential Git commands such as initializing repositories, staging files, committing changes, and pushing updates to GitHub.

The goal of this project is to build a strong foundation in reproducible and organized project management practices that are widely used in software development, data analysis, and research. This repository serves as a reference for future projects that require structured version control and collaboration.

---

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Setup](#setup)
- [Usage](#usage)
- [Credits](#credits)

---

## Introduction
**Git** is the version control system that tracks changes in your code.

**GitHub** is the platform where you can store your code in the cloud and collaborate with others.

**Version Control** is a system that records changes to a file or set of files over time.

**Repository** is the folder that stores your work. 

**Local Repository** is stored on your computer and contains all your project files and version history. It's where you make changes, stage, and commit your work.

**Remote Repository** like one hosted on GitHub, is stored online and acts as a shared version of your project for collaboration or backup. You push changes from your local repository to the remote, ensuring everyone working on the project has access to the latest version. Similarly, you pull updates from the remote to keep your local copy up to date.

**Commit** is a snapshot of changes made to files within a version control system, serving as a saved point in a project's history. It acts as a permanent record of a specific unit of work, allowing developers to track, compare, and revert to previous versions of the codebase.

---

## Installation and Setup

### Configuring GitHub with Git

You'll want to configure these settings:
1. User Identity
Git requires your name and email to label your commits, in your terminal follow the below commands:
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
2. Changing default Branch Name
Git typically defaults to master for new repositories. You can set it to main by default to be more in line with industry standards:
git config --global init.defaultBranch main

### Creating and updating a Github Repository
Initial Setup Steps

You will only need to run these steps once per project, the very first time you make each repository.

Create a local repository: This is your starting point to track changes in your project. If you've already created a local git repository, you can skip this step.

git init

Create a remote repository:

Go to GitHub.com and create a new repository by clicking the '+' icon in the top right hand corner on your dashboard.

Copy the remote URL.

Connect the local repository to the remote:

git remote add origin <github repository url>

- A remote, is the connection between your local git repository and your Github cloud repository- Origin, is the name of the remote. So, when we want to utilize this specific connection we will reference the name.

Push the work from your local repository to your cloud repository

git push origin main

A push is the act of sending the work in your local repository to your cloud repository.
We are referencing the origin remote so we can use that connection to our cloud repository.
main, is the name of the branch that we are going to be pushing. If you did not change your default branch from master to main then you will likely need to push the master branch.



---

## Usage

Staging a change is like preparing your work for review before submitting it. When you run git add ., you're telling Git, "These are the changes I want to include in my next update." Think of it as gathering your materials into a neat pile to be sent off. This step lets you double-check what's being tracked before you finalize it with a commit (git commit) and share it with your remote repository (git push).

You will run these steps every time you want to track changes to your repository:

git add .                      # Stage your changes
git commit -m "message"        # Commit changes with a message
git push origin <branch>       # Push changes to the remote repository



### Essential Git Commands

git status	
Shows the status of your repository.

git branch	
Lists all branches in your repository.

git checkout <branch>	
Switches to the specified branch.

git checkout -b <branch>	
Creates a new branch and switches to it.

git remote -v	


---

## Credits 
Coding Temple, Reddit 

