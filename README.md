# Git Commands Reference

This guide provides a reference for common Git commands along with their operations and examples.

## Git Commands:

1. **git init**:
   - **Operation**: Initialize a new Git repository.
   - **Example**:
     ```bash
     git init
     ```
     ![image](https://github.com/prathamesh78/Git/assets/104883046/d47fbad6-01f2-43b8-abc4-e3183f2c95ab)

2. **git add**:
   - **Operation**: Add file contents to the staging area
   - **Example**:
     ```bash
     git add <file_name>
     ```
     ![image](https://github.com/prathamesh78/Git/assets/104883046/437733c5-309c-4b67-b0bd-8013cfa710e0)

   - **Operation**: Add specific files to the staging area
   - **Example**:
     ```bash
     git add file <file_name1> <file_name2>
     ```
     ![image](https://github.com/prathamesh78/Git/assets/104883046/bd5375e4-f994-43e4-8fec-c11747773089)

   - **Operation**: Add specific type of files to the staging area
   - **Example**:
     ```bash
     git add *.doc
     ```
     ![image](https://github.com/prathamesh78/Git/assets/104883046/1ded7659-f6fd-431a-86bc-a3c29eec4675)

   - **Operation**: Add all the files to the staging area
   - **Example**
     ```bash
     git add .
     ```
     ![image](https://github.com/prathamesh78/Git/assets/104883046/ed9f946d-f455-4050-b272-d81fd1a3b66e)

3. **git rm**:
   - **Operation**: Remove the file from staging area to working directory
   - **Example**: 
     ```bash
     git rm --cached <file_name>
     ```
     ![image](https://github.com/prathamesh78/Git/assets/104883046/c3aa6a13-20c6-4ba9-a151-bd401ffda5c8)

   - **Operation**: Remove the file permanently from staging and working directory
   - **Example**:
     ```bash
     git rm -f <file_name>
     ```
     ![image](https://github.com/prathamesh78/Git/assets/104883046/2bc4d677-f216-4b3a-bb31-59c747a5d3e7)

4. **git commit**:
   - **Operation**: Record changes to the repository
   - **Example**:
     ```bash
     git commit -m "Commit message"
     ```
     ![image](https://github.com/prathamesh78/Git/assets/104883046/3096f53b-18a6-4b44-99f3-17cebcf53877)

5. **git status**:
    - **Operation**: Show the working tree status.
    - **Example**:
      ```bash
      git status
      ```
      ![image](https://github.com/prathamesh78/Git/assets/104883046/fd422e7b-4b10-4c8a-91c5-6a890efdb2c9)

6. **git log**:
   - **Operation**: Get the list of commit in the repository
   - **Example**:
     ```bash
     git log
     ```
     ![image](https://github.com/prathamesh78/Git/assets/104883046/7f1b460d-f364-4b0c-abfc-85a89e653683)

   - **Operation**: Get the list of last 'n' (n= number) commits in the repository
   - **Example**:
     ```bash
     git log -n
     ```
     ![image](https://github.com/prathamesh78/Git/assets/104883046/26a8f418-a63f-4a72-a61a-9ab1be04e3c2)
   
   - **Operation**: Get the list  of commit in single line
   - **Example**: 
     ```bash
     git log --oneline
     ```
     ![image](https://github.com/prathamesh78/Git/assets/104883046/b11f8daa-1d20-4811-9650-fdfa8606769e)

   - **Operation**: To get the summary of commits made and the number of changes
   - **Example**:
     ```bash
     git log --stat
     ```
     ![image](https://github.com/prathamesh78/Git/assets/104883046/c58d5f80-3f3c-487b-8a3c-028a4dba6d8a)

7. **git reset**
   - **Operation**: Undo the changes by commit
   - **Example**:
     ```bash
     git reset <commit_id>
     ```

   - **Operation**: Undo the changes from local repository to staging area and Changes will be available in both staging area and working directory.
   - **Example**:
     ```bash
     git reset --soft
     ```
     ![image](https://github.com/prathamesh78/Git/assets/104883046/4db7a375-c255-4e4d-ac64-a0ad94003eb5)
   
   - **Operation**: Undo the changes from local repository to working directory and the changes will be available in working directory and not in staging area  
   - **Example**:
     ```bash
     git reset --mixed
     ```
     ![image](https://github.com/prathamesh78/Git/assets/104883046/1a9121e2-a301-4a1e-a2a3-d9cd98497231)

   - **Operation**: Delete the  changes permanently from local repository, staging area as well as working directory
   - **Example**:
     ```bash
     git reset --hard
     ```
     ![image](https://github.com/prathamesh78/Git/assets/104883046/6b06258d-6554-4b35-8ad7-ec8608ae4da9)

     
8. **git clone**:
   - **Operation**: Clone a repository into a new directory.
   - **Example**:
     ```bash
     git clone <repository_url>
     ```

9. **git push**:
   - **Operation**: Update remote refs along with associated objects.
   - **Example**:
     ```bash
     git push origin master
     ```

10. **git pull**:
   - **Operation**: Fetch from and integrate with another repository or a local branch.
   - **Example**:
     ```bash
     git pull origin master
     ```

11. **git branch**:
   - **Operation**: List, create, or delete branches.
   - **Example**:
     ```bash
     git branch feature_branch
     ```

12. **git checkout**:
   - **Operation**: Switch branches or restore working tree files.
   - **Example**:
     ```bash
     git checkout feature_branch
     ```

13. **git merge**:
   - **Operation**: Join two or more development histories together.
   - **Example**:
     ```bash
     git merge feature_branch
     ```

