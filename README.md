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

8. **git revert**:
   - **Operation**: To revert the changes at a specific commit. It is same as git reset --hard 
   - **Example**:
     ```bash
     git revert <commit_id>
     ```
     ![image](https://github.com/prathamesh78/Git/assets/104883046/947ce939-e5a4-44e9-9b8a-9926b51fef10)
     ![image](https://github.com/prathamesh78/Git/assets/104883046/c2cc9629-2a64-4673-a6b5-559f3d5490ab)

9. **git ignore**: It is used to ignore the files/folders in the git repository from tracking
   - **Operation**: create a repository, Initialize the repository, create .gitignore file and add the files and folders which you want to ignore
     ![image](https://github.com/prathamesh78/Git/assets/104883046/ad706b81-36fc-4f1e-bf8b-71ac7e20da6c)
     ![image](https://github.com/prathamesh78/Git/assets/104883046/ce8fdab9-4e88-43c0-bed1-5fcb86dd0912)

 10. **git branch**:
     - **Operation**: List, create, or delete branches.
     - **Example**:
       ```bash
       git branch feature_branch
       ```
       
     - **Example**:
       ```bash
       git switch -c <feature_branch>
       ```
   
     - **Example**:
       ```bash
       git switch <master>
       ```
   
     - **Example**:
       ```bash
       git checkout -b <feature_branch>
       ```
   
     - **Example**:
       ```bash
       git branch -d <feature_branch>
       ```
       ![image](https://github.com/prathamesh78/Git/assets/104883046/882896dc-158a-4af1-93e0-0c9a92f2a8e2)

11. **git merge**:
    - **Operation**: Join two or more development histories together.
    - **Example**:
      ```bash
      git merge feature_branch
      ```
      ![image](https://github.com/prathamesh78/Git/assets/104883046/6f05ef14-1392-4a58-8f8b-df50597f571f)
    - **Operation**: Conflict resolution of branches
    - **Solution**: Identify the file(s) causing the issue in target branch, Open the file and review the file content, Decide which record has to be retained/deleted, Remove the header and footer, Update the file content, add the changes and commit the changes in target branch.

      ![image](https://github.com/prathamesh78/Git/assets/104883046/e64d641d-d852-4663-9732-24ee0cac0245)

      ![image](https://github.com/prathamesh78/Git/assets/104883046/db622449-f7da-4a92-9d65-3466a2734faa)

      ![image](https://github.com/prathamesh78/Git/assets/104883046/ed507536-815a-4f8a-ae69-d17b8e5c1c8c)

12. **git rebase**:
    - **Operation**: To maintain linear commit history
    - **Example**:
      ```bash
      git rebase <target_branch>
      ```
      ![image](https://github.com/prathamesh78/Git/assets/104883046/ffb00c2f-ae56-428f-aa2a-0a60f63e3ce2)

13. **git squash**:
    - **Operation**: To combine more that one commit and create a new commit point.
    - **Example**:
      ```bash
      git merge --squash <branch>
      ```

      ![image](https://github.com/prathamesh78/Git/assets/104883046/aea98389-3238-4d5c-baa5-17c373c3ad1f)

      ![image](https://github.com/prathamesh78/Git/assets/104883046/b0c6776f-497f-414d-b1a6-8322853cd673)

      ![image](https://github.com/prathamesh78/Git/assets/104883046/5de19f20-3edd-4071-81ba-690bf9ad3473)

14. **Rename the Branch**:
    - **Operation**: Rename the Branch name
    - **Example**:
      ```bash
      git branch -M <branch_name>
      ```

14. **git stash**:
    - **Operation**: To save the uncommited changes to a temporary area.
    - **Example**:
      ```bash
      git stash save "commit message"
      ```
      ![image](https://github.com/prathamesh78/Git/assets/104883046/df069679-997b-4072-afda-a54c599eb9cd)

    - **Operation**: To get the list of stashed entries.
    - **Example**:
      ```bash
      git stash list
      ```
      ![image](https://github.com/prathamesh78/Git/assets/104883046/42ffd244-a558-46cd-bbc4-15a9a47ac253)

    - **Operation**: To apply the latest entry from the stash list, back to staging area.
    - **Example**:
      ```bash
      git stash apply
      ```
      ![image](https://github.com/prathamesh78/Git/assets/104883046/dfa69d93-ddc7-456d-b8fa-f6ea0f8f0d16)
   
    - **Applying for specific entry**
      ```bash
      git stash apply stash@{1}
      ```
      ![image](https://github.com/prathamesh78/Git/assets/104883046/3a42d86c-f06a-446b-a343-5b240c204afc)

    - **Operation**: To delete/drop the latest entry from the stash list
    - **Example**:
      ```bash
      git stash drop
      ```
      ![image](https://github.com/prathamesh78/Git/assets/104883046/c528c998-aee9-4575-84a1-e593cb1b16ca)

    - **Drop a specfic entry**
      ```bash
      git stash drop stash@{1}
      ```
      ![image](https://github.com/prathamesh78/Git/assets/104883046/18e1e305-9767-4708-a057-09e8f242facf)

    - **Operation**: To apply the latest entry from the stash list, back to staging area as well as remove that entry from the stash list.
    - **Example**:
      ```bash
      git stash pop
      ```
      ![image](https://github.com/prathamesh78/Git/assets/104883046/f110d6a9-086e-4ef6-8530-c77beced054a)

    - **pop specfic entry**
      ```bash
      git stash pop stash@{0}
      ```
      ![image](https://github.com/prathamesh78/Git/assets/104883046/1b331de1-702e-4544-b833-df391b2ca04a)

    - **Clear a stash list**
      ```bash
      git stash clear
      ```
      ![image](https://github.com/prathamesh78/Git/assets/104883046/4efd436d-027d-40df-a9ba-62275b432f2a)
                      
15. **git clone**:
    - **Operation**: Clone a repository into a new directory.
    - **Example**:
      ```bash
      git clone <repository_url>
      ```
      ![image](https://github.com/prathamesh78/Git/assets/104883046/05f346e7-74b5-4606-9396-81946f445c41)

16. **git remote**:
    - **Operation**: To get the list of remote repository linked to the local repository
    - **Example**:
      ```bash
      git remote -v
      ```
      ![image](https://github.com/Prathamesh78/Git/assets/104883046/e62d7367-8586-4b85-b946-daefdb9eb506)
   
17. **git push**:
    - **Operation**: To push the changes to the remote repository using the credentials
    - **Example**:
      ```bash
      git push -u origin <branch_name>
      ```
      ![image](https://github.com/Prathamesh78/Git/assets/104883046/0f295c71-b288-4130-a2aa-d79fc26318d6)

      ![image](https://github.com/Prathamesh78/Git/assets/104883046/4d304bc1-364d-4857-acca-1bd907d41200)

      ![image](https://github.com/Prathamesh78/Git/assets/104883046/64bf12d9-8032-48b1-874d-b404a33fc934)
 
18. **git fetch**:
    - **Operation**: To check for the incremental changes and if there are any changes exist in the remote repository, it will update the changes in the local repository. NOT in the Working Directory.
    - **Example**:
      ```bash
      git fetch
      ```
      ![image](https://github.com/Prathamesh78/Git/assets/104883046/0b885650-165d-436a-9ee7-618432ae87f6)

19. **git pull**:
    - **Operation**: To check for the incremental changes and if there are any changes exist in the remote repository, it will update the changes in the local repository as well as in the Working Directory
    - **Example**:
      ```bash
      git pull 
      ```
      ![image](https://github.com/Prathamesh78/Git/assets/104883046/7852fdf4-9e23-43dd-836a-419f0b593895)
