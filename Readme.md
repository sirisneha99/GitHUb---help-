This a quick handook of git bash commands and useful tips to getting started with github.


1. mkdir folder_name  -> creates a directory (using the git bash shell)

2. cd folder/file_name -> takes you to the specified file/folder name

3.pwd -> shows you the directory / folder that you are currently working in ( is short for print working directory) 

4. git clone  HTTPS_link_of_repo -> clones you the repo in your local machine from github using HTTPS

5. git status -> gives u the status of the repo - telling if any changes need to be committed. Always a good  practice to check the status before adding/ removing files from the repository

6. touch file_name - creates a new file

7. git add file_name -> adds a file into the repository. Now the git can track the changes made to the file. Earlier when the file was creaetd using "touch", git didn't hhave access to track the file

8. git restore --stage file_name -> to revert the tracking system, now, altough the file is in the repository, the git cannoyt track the file any longer

9. git commit -m "message" -> use this command once you are done with the staging process(after adding/ removing/updating files). This helps in finalising the code into actual program. Th -m flag is used to type a message 

   NOTE - Using commit,all changes are made only on the local machine. In order to make changes global( in the remote server, which is the server available for other s to access via github), you need to use the Push command(due to git being DVCS)

   * A good practice is to use pwd and git status before starting to make changes to your repository
  
10. git checkout - B branch_name -> creates a new beanch and also takes you to the branch, so you can readily start uodating changes
11. git branch branch_name -> creates a new branch; alsi shows which branch you are currentky working on
    NOTE - The changes made in the branch is not shown in the main branch. The main branch is completely unaware of these changes. Git branches exist in isolation. Changes need to be merged back into the main branch. We use git push to update the changes made in the remote repository which can be accessed via github

12. git push -u origin branch_name/file/directory_name -> using the -u flag helps in knowing the updates from the upstream - which in this case is the main branch. Now the main branch would be the specified branch name
13. Once the commited code is pushed, a pull request is cfreated in the remote repository(github) for other devs to review and approve the code befor merging the branch into main branch.
14. Branching is beneficial as the approach of keeping everything at branch leverl is much easier than having everyone working at the main line as it casues issues. Having independent branches is easier to manage and there's no limit to how many branches we can have.When adding a new feature, the branch can be named - feature/feature_name. When fixing a bug, banch can be named as - fix / bug_name
15. After the pull request is validated, a merge option is provided.
16. Once merged, you can delete or keep the merged branch
17. git checkout main -> To see the status of the main branch
18. git pull -> to see the recent updates in your repo
19. ls -> lists all files inside your repo/ dir
20. 
