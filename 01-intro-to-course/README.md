#01-intro-to-course

# Introduction to Fullstack Development Course

Welcome to the Fullstack Development Course! This course is designed to provide you with a comprehensive understanding of the technologies and tools used in modern web development. Whether you're a beginner or have some experience in web development, this course will equip you with the skills to build robust and scalable full-stack applications.

# Code Editor Setup

To get started, you'll need to set up a code editor on your computer. We recommend using Visual Studio Code (VS Code) as it's a popular and versatile editor that supports various programming languages and has a wide range of extensions for different purposes.

# Git Basics for Fullstack Development Course

## What is Git?

Git is a distributed version control system that tracks changes in your code over time. It allows developers to:

- Keep a history of all changes made to their codebase
- Revert to previous versions if needed
- Work on different features simultaneously without interfering with each other
- Collaborate with other developers efficiently
- Maintain multiple versions of the same project

Git works by taking "snapshots" of your files whenever you make a commit, creating a timeline of your project's development that you can navigate through.

## Git vs. GitHub: Understanding the Difference

**Git** is the version control system itself - the tool that tracks changes to your files on your local machine. It operates completely independently and doesn't require an internet connection.

**GitHub** is a cloud-based hosting service for Git repositories. It adds a visual interface and additional features on top of Git, including:

- A central location to store your repositories online
- Tools for code review and project management
- Issue tracking
- Pull requests for collaborative development
- Actions for continuous integration/deployment
- Social features to discover and contribute to other projects

In simple terms: Git is the tool, GitHub is a service built around that tool.

## Installing Git

1. Download the installer from [git-scm.com](https://git-scm.com/downloads)
2. Run the installer, accepting the default options (you can customize if you're familiar with the settings)
3. Open Command Prompt or Git Bash to verify installation:
   ```bash
   git --version
   ```
   After installing Git, set up your identity:

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

This information will be associated with any commits you make.

## Staying Updated with the Course Repository

To follow along with the course and get updates as new content is added, follow these steps:

### Initial Setup (One-time)

1. Clone the course repository:
   ```bash
   git clone https://github.com/ShalevAsor/Learn-Fullstack.git
   cd Learn-Fullstack
   ```

### Getting Updates for the Course Material

Whenever you want to check for and download new course content:

1. Navigate to your local repository:

   ```bash
   cd path/to/Learn-Fullstack
   ```

2. Fetch the latest changes from the remote repository:

   ```bash
   git fetch origin
   ```

   OR

3. Pull the latest updates from the main branch:
   ```bash
   git pull origin main
   ```

### Working on Your Own Version

Since you cannot push changes directly to the course repository, here's how to work on your own version of the project:

#### Option 1: Create a Local Branch

This lets you make changes locally while still being able to get updates:

```bash
# Create and switch to a new branch for your work
git checkout -b my-work

# Now you can make changes without affecting the main branch
# When you want to get course updates:
git checkout main
git pull origin main

# Then return to your work branch and merge in the updates
git checkout my-work
git merge main
```

#### Option 2: Fork the Repository (Recommended)

For a more complete experience similar to real-world development:

1. On GitHub, navigate to [https://github.com/ShalevAsor/Learn-Fullstack](https://github.com/ShalevAsor/Learn-Fullstack)
2. Click "Fork" in the upper right to create your own copy
3. Clone your fork to your computer:
   ```bash
   git clone https://github.com/YOUR-USERNAME/Learn-Fullstack.git
   cd Learn-Fullstack
   ```
4. Add the original repository as a remote to get updates:
   ```bash
   git remote add upstream https://github.com/ShalevAsor/Learn-Fullstack.git
   ```
5. Now you can get updates while keeping your work:

   ```bash
   # Get updates from the course repository
   git fetch upstream
   git merge upstream/main

   # Push your work to your fork
   git push origin main
   ```

This way, you'll be able to follow along with the course material while also creating your own version of the project that you have full control over.

Throughout this course, I'll be updating the repository with new material. Using these commands will ensure you always have the latest content while maintaining your own work.
