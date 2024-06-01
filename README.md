# Using TS-Quickstart-Template for Node.js projects

This repository is for quickly starting up a typescript Node.js project. If you have any modifications please contribute!

## Part 1: Cloning and setting up your own Github repository

(if you don't want to have a remote repository or a repository at all, skip to step #2)

### Part 1: Clone the Existing Repository with a New Directory Name

Clone the existing repository to your local machine and specify the new directory name:

```sh
git clone https://github.com/Frankovich/TS-Quickstart-Template.git new_repo_name
cd new_repo_name
```

### 2. Remove the Existing Git History

Remove the existing Git history to start fresh:

```sh
find . -name ".git" -type d -exec rm -rf {} +
```

### 3. Initialize a New Git Repository

Initialize a new Git repository in the directory:

```sh
git init
```

### 4. Add Files to the New Repository

Add all your project files to the staging area:

```sh
git add .
```

### 5. Commit the Files

Commit the files to the new repository:

```sh
git commit -m "Initial commit"
```

### 6. Create a New Repository on GitHub

Go to GitHub and create a new repository. Do not initialize it with a README, .gitignore, or license. Note the repository URL for the next step.

### 7. Add the New GitHub Repository as a Remote

Add your new GitHub repository as a remote to your local repository. Replace `user_name/your_repo` with your GitHub username and repository name:

```sh
git remote add origin https://github.com/user_name/your_repo_name.git
```

### 8. Push the Commit to GitHub

Push your commit to the new GitHub repository:

```sh
git push -u origin master
```

## Part 2: Dependencies

### 1. Install Project Dependencies

Navigate to your project directory and install the required dependencies:

```sh
npm install ts-node typescript @types/node --save-dev
```

### 2. Install Node Modules

Install all dependencies specified in `package.json`:

```sh
npm install
```

### 3. Start the Project

Run your project using the start script:

```sh
npm start
```

This setup will ensure that your TypeScript project is correctly configured and ready for development.
