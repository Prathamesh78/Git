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
   - **Operation**: Add specific files to the staging area
   - **Example**:
     ```bash
     git add file <file_name1> <file_name2>
     ```
   - **Operation**: Add specific type of files to the staging area
   - **Example**:
     ```bash
     git add *.doc
     ```
   - **Operation**: Add all the files to the staging area
   - **Example**
     ```bash
     git add .
     ```
		
3. **git rm**
   - **Operation**: Remove the file from staging area to working directory
   - **Example**: 
     ```bash
     git rm --cached <file_name>
     ```
   - **Operation**: Remove the file permanently from staging and working directory
   - **Example**:
     ```bash
     git rm -f <file_name>
     ```

4. **git commit**:
   - **Operation**: Record changes to the repository
   - **Example**:
     ```bash
     git commit -m "Commit message"
     ```
5. **git log**:
   - **Operation**: Get the list of commit in the repository
   - **Example**:
     ```bash
     git log
     ```

   - **Operation**: Get the list of last 'n' (n= number) commits in the repository
   - **Example**:
     ```bash
     git log -n
     ```
   
   - **Operation**: Get the list  of commit in single line
   - **Example**: 
     ```bash
     git log --oneline
     ```

   - **Operation**: To get the summary of commits made and the number of changes
   - **Example**:
     ```bash
     git log --stat
     ```

6. **git reset**
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
   
   - **Operation**: Undo the changes from local repository to working directory and the changes will be available in working directory and not in staging area  
   - **Example**:
     ```bash
     git reset --mixed
     ```

   - **Operation**: Delete the  changes permanently from local repository, staging area as well as working directory
   - **Example**:
     ```bash
     git reset --hard
     ```
     
3. **git clone**:
   - **Operation**: Clone a repository into a new directory.
   - **Example**:
     ```bash
     git clone <repository_url>
     ```


5. **git push**:
   - **Operation**: Update remote refs along with associated objects.
   - **Example**:
     ```bash
     git push origin master
     ```

6. **git pull**:
   - **Operation**: Fetch from and integrate with another repository or a local branch.
   - **Example**:
     ```bash
     git pull origin master
     ```

7. **git branch**:
   - **Operation**: List, create, or delete branches.
   - **Example**:
     ```bash
     git branch feature_branch
     ```

8. **git checkout**:
   - **Operation**: Switch branches or restore working tree files.
   - **Example**:
     ```bash
     git checkout feature_branch
     ```

9. **git merge**:
   - **Operation**: Join two or more development histories together.
   - **Example**:
     ```bash
     git merge feature_branch
     ```

10. **git status**:
    - **Operation**: Show the working tree status.
    - **Example**:
      ```bash
      git status
      ```
