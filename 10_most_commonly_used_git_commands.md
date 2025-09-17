# 10 Most Commonly Used Git Commands

Git is a powerful version control system widely used in software development. Here are 10 of the most commonly used Git commands:

1. **git init**
   - Initializes a new Git repository in the current directory.
   - Example:  
     ```bash
     git init
     ```

2. **git clone**
   - Copies an existing repository from a remote server (like GitHub) to your local machine.
   - Example:  
     ```bash
     git clone https://github.com/user/repo.git
     ```

3. **git status**
   - Shows the current status of your working directory and staging area.
   - Example:  
     ```bash
     git status
     ```

4. **git add**
   - Adds changes in your working directory to the staging area, preparing them for a commit.
   - Example:  
     ```bash
     git add filename.txt
     git add .
     ```

5. **git commit**
   - Records changes in the repository with a descriptive message.
   - Example:  
     ```bash
     git commit -m "Add new feature"
     ```

6. **git push**
   - Uploads local commits to a remote repository.
   - Example:  
     ```bash
     git push origin main
     ```

7. **git pull**
   - Fetches and merges changes from a remote repository to your local branch.
   - Example:  
     ```bash
     git pull origin main
     ```

8. **git branch**
   - Lists all branches or creates a new branch.
   - Example:  
     ```bash
     git branch        # list branches
     git branch new-feature  # create a new branch
     ```

9. **git checkout**
   - Switches between branches or restores files.
   - Example:  
     ```bash
     git checkout main
     git checkout -b new-feature  # create and switch to a new branch
     ```

10. **git merge**
    - Merges changes from one branch into another.
    - Example:  
      ```bash
      git merge new-feature
      ```

