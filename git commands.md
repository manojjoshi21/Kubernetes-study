git commands

1. Create repository

 mkdir myproject1
 cd myproject1
 git init

 now repository is created

 2.  create index.html file and store in the directory . If u hit ls we can see files
     Now Git is aware of the file, but has not added it to our repository!

     Files in your Git repository folder can be in one of 2 states:

    Tracked - files that Git knows about and are added to the repository
    Untracked - files that are in your working directory, but not added to the repository
    When you first add files to an empty repository, they are all untracked. To get Git to track them, you need to stage them, or add them to the staging environment.

3. Git Staging Environment
One of the core functions of Git is the concepts of the Staging Environment, and the Commit.

As you are working, you may be adding, editing and removing files. But whenever you hit a milestone or finish a part of the work, you should add the files to a Staging Environment.
Staged files are files that are ready to be committed to the repository you are working on

4.  git add index.html -- so that the file is moved to staging and getting tracked
    now you can check using  git status

5.  If there are multiple files you can add git add - all

6. ...