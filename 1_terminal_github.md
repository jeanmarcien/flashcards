# Flashcards: Ruby & Github

## Flashcard 1
**Q:**
- How do I check my current directory?

**A:**
- Use the `pwd` command. It prints the path of your current directory.
  ```bash
  pwd
  ```
---

## Flashcard 2
**Q:**
- How do I list files in my current directory?

**A:**
- Use the `ls` command. Add `-lh` for detailed information
  ```bash
  ls
  ls -lh
  ```
---

## Flashcard 3
**Q:**
- How do I move between directories?

**A:**
- Use the `cd` command to go into a folder:
  ```bash
  cd <FOLDER_NAME>
  ```
- Use the `cd` command to go up one evel:
  ```bash
  cd ..
  ```
---

## Flashcard 4
**Q:**
- How do I create a new folder or file?

**A:**  
- Create a directory:
  ```bash
  mkdir <NEW_FOLDER>
  ```
- Create a file:
  ```bash
  touch <FILE_NAME>
  ```
---

## Flashcard 5
**Q:**  
- How do I view the content of a text file?

**A:**  
- Use the `cat` command:
  ```bash
  cat <FILE_NAME>
  ```
- Tip: Use `code .` to open the current folder in your text editor.
---

## Flashcard 6 
**Q:**  
- How do I move or rename files?

**A:**  
- Use the `mv` command to move a file:
```bash
mv <FILE_NAME> <FOLDER_NAME>
```
- Use the `mv` command to rename a file:
```bash
mv <FILE_NAME> <NEW_FILENAME>
```
---

## Flashcard 7  
**Q:**  
- How do I start a Git repository or clone an existing one?

**A:**  
- Initialize a new Git repository:
  ```bash
  git init
  ```
- Clone a repository from Github:
  ```bash
  git clone <GITHUB_SSH_CLONE_URL>
  ```
---

## Flashcard 8  
**Q:**  
- How do I check the current state of my repository?

**A:**  
- Use `git status` to see changes, staged files, and untracked files.
  ```bash
  git status
  ```
---

## Flashcard 9  
**Q:**  
- How do I commit my changes in Git?

**A:**  
- First, add files to the staging area:
  ```bash
  git add <FILE_NAME>
  ```
- Finally, commit the staged files with a message:
  ```bash
  git commit -m "Your meaningful message"
  ```
---

## Flashcard 10  
**Q:**  
- How do I push changes to GitHub?

**A:**
- Ensure your repository is connected to GitHub and use `git push`:
  ```bash
  git push origin master
  ```
