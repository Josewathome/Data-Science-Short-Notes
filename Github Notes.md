
---

## **Setting Up Git and GitHub with Git Bash**

1. **Configure Git User Details**:
   ```bash
   git config --global user.name "your username"
   git config --global user.email "email@gmail.com"
   git config --global init.defaultBranch main
   ```

2. **Navigate to Your Project Directory**:
   ```bash
   cd C:/path/to/your/project
   ```

3. **Initialize a Git Repository**:
   ```bash
   git init
   ```

   > If you encounter a "not safe directory" error, use:
   ```bash
   git config --global --add safe.directory "C:/path/to/your/project"
   ```

---

## **Basic Git Commands**

### **Check Repository Status**
```bash
git status
```

### **Track Files**
- Add a single file:
  ```bash
  git add <filename>
  ```
- Add all files:
  ```bash
  git add --all
  # or
  git add -A
  # or
  git add .
  ```

### **Unstage Files**
- Remove a file from staging:
  ```bash
  git rm --cached <filename>
  ```

### **Commit Changes**
- Save the current state of your repository:
  ```bash
  git commit -m "Commit message here"
  ```
- Commit and add all changes directly:
  ```bash
  git commit -a -m "Commit message here"
  ```

---

## **Ignoring Files**

1. Create a `.gitignore` file in your project directory.
2. Add files or patterns to ignore:
   ```
   # Comments start with #
   *.log
   node_modules/
   ```
3. Save the file and verify:
   ```bash
   git status
   ```

---

## **Checking Changes**

- View changes in files:
  ```bash
  git diff
  ```

- View the commit log:
  ```bash
  git log
  ```
- View a simplified log:
  ```bash
  git log --oneline
  ```

---

## **Branches**

1. **Create a Branch**:
   ```bash
   git branch <branch-name>
   ```
2. **Switch Between Branches**:
   ```bash
   git switch <branch-name>
   ```
3. **Merge a Branch into the Current Branch**:
   ```bash
   git merge <branch-name>
   ```
4. **Delete a Branch**:
   ```bash
   git branch -d <branch-name>
   ```

---

## **Resolving Merge Conflicts**

1. After attempting a merge, if there’s a conflict:
   ```bash
   git merge <branch-name>
   ```
2. Open the conflicted files and resolve the issues.
3. Add the resolved files:
   ```bash
   git add <filename>
   ```
4. Commit the resolution:
   ```bash
   git commit -m "Resolved merge conflict"
   ```

---

## **Working with GitHub**

### **Push to GitHub**
1. Add a remote repository:
   ```bash
   git remote add origin <repository-URL>
   ```
2. Set the default branch:
   ```bash
   git branch -M main
   ```
3. Push to GitHub:
   ```bash
   git push -u origin main
   ```
4. Push all branches:
   ```bash
   git push --all
   ```

### **Pull Changes from GitHub**
```bash
git pull
```

---

## **Adding a README.md**
Create a `README.md` file:
```bash
echo "# Your Project Title" >> README.md
```

---
