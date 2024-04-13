***States in GIT***:-  

**Working Directory**: 

  This is where you make modifications to your files. 

  Files in this state are considered to be in the "untracked" or "modified" state. 

**Staging Area (Index):** 

  After making changes in the working directory, you use the git add command to stage these changes. 

  Staging allows you to group related changes together before committing them. 

  Files in this state are considered to be in the "staged" state. 

**Local Repository:** 

  After staging your changes, you use the git commit command to save them permanently to the Git repository. 

  Files in this state are considered to be in the "committed" state. 

levels of configuration in GIT:- 

- Repository (Local):- 
  - Stored in "/g/Automation Testing/git\_commands/.git/config" 
  - These settings are specific to a single Git repository. 
  - They are stored in the .git/config file within the repository. 
  - Local configurations override global configurations for that specific repository. 
  - You can view and edit local-level configurations directly by opening the .git/config file or by using the git config command without any flag, which automatically refers to the local configuration for the current repository.
    
- User Account (Global):- 
  - Stored in - "~/.gitconfig" 
  - These settings are specific to a particular user on the system and apply to all Git repositories for that user. 
  - They are stored in the user's home directory, usually in the .gitconfig file. 
  - You can view and edit global-level configurations using the git config command with the --global flag. 
  - git config --global --edit
  
- System Level (Git Installation) :-  
  - Stored in - "/etc/gitconfig"  
  - These settings apply to the entire Git system and are shared among all users on the machine. 
  - They are stored in the gitconfig file within the Git installation directory.  
  - You can view and edit system-level configurations using the git config command with the --system flag.
  - git config --system --edit 

**Config user name and password** 
![image](https://github.com/AishwaryaDhotre21/design-automation-framework/assets/83119495/bfa70891-7535-48d6-8155-5d546032f362)

![image](https://github.com/AishwaryaDhotre21/imp-docs/assets/83119495/f7026d46-6d49-4030-bead-3049872f2eee)

![image](https://github.com/AishwaryaDhotre21/imp-docs/assets/83119495/3ae8b77e-2e40-40eb-b144-c84d4ee13e22)


- The priority of configuration levels is such that local configurations take precedence over global configurations, which, in turn, take precedence over system configurations

![image](https://github.com/AishwaryaDhotre21/imp-docs/assets/83119495/2e794bf5-cde2-48e1-87ee-6b3da55da758)



**Git Commands** 

- Git help
![image](https://github.com/AishwaryaDhotre21/imp-docs/assets/83119495/a1ba11a8-b4e7-4017-b8a0-cb345ddf0bb8)


- Git init
![image](https://github.com/AishwaryaDhotre21/imp-docs/assets/83119495/a7607919-31e0-47bd-a603-f834c57f31c5)



- Git status 
![image](https://github.com/AishwaryaDhotre21/imp-docs/assets/83119495/06703751-960a-4373-86c0-4cd85a611dc8)



- Git add 
![image](https://github.com/AishwaryaDhotre21/imp-docs/assets/83119495/2bad2a46-579e-4e80-b6b7-5299d462121b)

  ![image](https://github.com/AishwaryaDhotre21/imp-docs/assets/83119495/f64e293b-f62d-4726-8d96-6f972bd56d75)



- Git commit 
![image](https://github.com/AishwaryaDhotre21/imp-docs/assets/83119495/947e1a12-cf6d-4750-8e33-88b3354aae00)

  ![image](https://github.com/AishwaryaDhotre21/imp-docs/assets/83119495/8ee72f15-6150-4fc0-b038-d70fae89cdbf)



- Git diff: - compare the changes in the  working area & staged area
![image](https://github.com/AishwaryaDhotre21/imp-docs/assets/83119495/ce928231-cd28-491f-ad9b-383223dd6a8e)




- Git diff –staged: - compare the changes in the staged area and repository area 
![image](https://github.com/AishwaryaDhotre21/imp-docs/assets/83119495/6e4f3fd2-65df-4568-b102-b851b43f4162)



- Git diff head:-   compare the changes in the working area and repository area 
![image](https://github.com/AishwaryaDhotre21/imp-docs/assets/83119495/2d23f452-ff64-46df-946f-06304e78d983)



- Git restore: command is used to restore working tree files. It's primarily used for manipulating the state of files in the working directory or the index (staging area).
![image](https://github.com/AishwaryaDhotre21/imp-docs/assets/83119495/fd67b4bb-e6d2-484a-b66a-dfea6565026d)



- Git restore –staged 
![image](https://github.com/AishwaryaDhotre21/imp-docs/assets/83119495/887c6506-da27-4440-b5e9-9277bae2c07a)



- Git branching 
  - Git checkout -b branch1 
  - Git branch 
![image](https://github.com/AishwaryaDhotre21/imp-docs/assets/83119495/d2613a65-ee23-42e8-b4f5-79af097cd133)



- Git rebase branch-name - rebase doesn’t add the extra commit.  
- Git merge branch-name - merge the desired branch into the current branch & add one extra merge commit 
![image](https://github.com/AishwaryaDhotre21/imp-docs/assets/83119495/2d904ae6-8421-4b6d-b60c-e7cdeb7be80a)



- Git commit  --amend : – change the latest commit 
- Git cherry-pick hash – apply specific commit from one branch to another branch
![image](https://github.com/AishwaryaDhotre21/imp-docs/assets/83119495/b815cb72-99b2-4ef7-8b3b-0975f1c0d8be)



- Git stash save “stash-name”– save the changes in the working directory to stash
![image](https://github.com/AishwaryaDhotre21/imp-docs/assets/83119495/d29b2fcb-ea91-4d82-9351-b5c13c6dd5ab)

- Git stash pop – remove & apply the stash from the stash list
![image](https://github.com/AishwaryaDhotre21/imp-docs/assets/83119495/18e629cd-3163-411f-981e-18443d74c2f5)
 
- Git stash apply - apply the stash without removing it from the stash list
![image](https://github.com/AishwaryaDhotre21/imp-docs/assets/83119495/43117028-d7b7-41f5-a907-fb36bb51208a)
 
- Git stash list – list the contents in the stash 
- git stash apply stash@{1} – apply the specific stash
![image](https://github.com/AishwaryaDhotre21/imp-docs/assets/83119495/a63c1df6-df01-4ce9-967c-207c6dfd7709)



- Git  reset :-  default flag is mixed 
  - Soft  : Moves the branch pointer to the specified commit.Leaves the changes staged (changes will not be lost). keeps the changes in te working directory as it is .
  ![image](https://github.com/AishwaryaDhotre21/imp-docs/assets/83119495/97b9f1cc-e02f-463c-b885-914808b6c870)
  
  - Mixed : Moves the branch pointer to the specified commit.Unstages the changes (changes are not lost). keeps the changes in te working directory as it is .
  ![image](https://github.com/AishwaryaDhotre21/imp-docs/assets/83119495/b8d4da94-a588-4f65-b9a9-d26725c249c1)
  
  - Hard : Moves the branch pointer to the specified commit.Discards all changes (working directory and staging area). 
  ![image](https://github.com/AishwaryaDhotre21/imp-docs/assets/83119495/7ccd9308-fb5a-428e-ab52-e8898472a246)



- Git reflog - This command will show a list of recent actions and their corresponding commit hashes and references. It's a useful tool for tracking changes and can be particularly handy for recovering lost commits or branches. 






**Push changes to remote repository:-** 

1. Create github repo
2. Generate ssh keys
3. Add public key to github
4. Initialize the git in the working repository  
  - Start ssh-agent.exe service 
  - Add private key to ssh-agent 
![image](https://github.com/AishwaryaDhotre21/imp-docs/assets/83119495/530c959e-8875-42a3-b74b-67d223063beb)
  ![image](https://github.com/AishwaryaDhotre21/imp-docs/assets/83119495/c1c01013-7620-405d-945b-194864984f10)



- Authenticate with github
![image](https://github.com/AishwaryaDhotre21/imp-docs/assets/83119495/ad55e0fd-db11-49e3-b496-b28127230768)



- Add remote url
![image](https://github.com/AishwaryaDhotre21/imp-docs/assets/83119495/be826274-4996-4072-93f1-10002caa5a44)

  ![image](https://github.com/AishwaryaDhotre21/imp-docs/assets/83119495/bee969d4-bf86-48e2-b59e-3f064d5a32e9)


- Rebase the remote branch on local branch
![image](https://github.com/AishwaryaDhotre21/imp-docs/assets/83119495/aa558122-a737-416c-8f47-ec4c5ce22f7d)

- Check the branches
![image](https://github.com/AishwaryaDhotre21/imp-docs/assets/83119495/e13b4410-d4a7-4129-a581-26ab7d4137cb)


- Pull the changes from remote repo
![image](https://github.com/AishwaryaDhotre21/imp-docs/assets/83119495/c01195f5-929a-48a3-aa62-c92fcd1538e0)


- Push the code
![image](https://github.com/AishwaryaDhotre21/imp-docs/assets/83119495/fd49c686-08fd-43f6-8712-3c0899748878)















# *Revert:*

- Purpose: The git revert command is used to create a new commit that undoes the changes introduced by a specific commit or range of commits. It's primarily used for reverting changes that have already been committed to the repository.

- Workflow: When you revert a commit, Git creates a new commit that represents the inverse of the changes introduced by the reverted commit. This maintains a clear history and does not alter the existing commit history. It's a safe way to undo changes without rewriting history, making it suitable for shared branches.

# *Restore:*

- Purpose: The git restore command is used to restore working tree files. It's primarily used for manipulating the state of files in the working directory or the index (staging area).

- Workflow: When you restore a file, you're typically restoring it to a previous state, either from the index (staging area) or from a previous commit. Unlike revert, restore operates on the working directory and staging area, but it doesn't create new commits.


## Key Differences:

Scope:

- revert operates at the commit level, creating new commits to undo changes introduced by specific commits.
- restore operates at the file level, restoring files in the working directory or staging area to a previous state.

Effect on History:

- revert preserves commit history by creating new commits to undo changes, ensuring that the original commits remain in the history.
- restore does not affect commit history; it only modifies the state of files in the working directory or staging area.
  
Safety:

- revert is safer for shared branches because it doesn't rewrite history and allows collaborators to see what changes were undone.
- restore is more immediate and local, making it suitable for manipulating files in your working directory or staging area without affecting other users.
  
*In summary, revert is used to undo changes at the commit level while preserving history, while restore is used to manipulate the state of files in the working directory or staging area without creating new commits.*







# *Merge:*

*Purpose:*
- The git merge command combines changes from one branch into another branch. It creates a merge commit to tie together the histories of the merged branches.

*Workflow:*
- When you merge branches, Git creates a new commit that represents the combination of changes from the merged branches. This results in a merge commit that has two or more parent commits, showing where the branches diverged and were merged.

*Commit History:*
- Merging preserves the commit history of both branches, including their individual commit timelines. Merge commits explicitly indicate when and where branches were merged.

Usage:

git checkout <branch_to_merge_into>

git merge <branch_to_merge_from>


# *Rebase:*

*Purpose:*
- The git rebase command integrates changes from one branch into another by reapplying commits on top of another branch. It rewrites the commit history of the rebased branch.

*Workflow:*
- When you rebase a branch, Git applies the commits from the rebased branch on top of the target branch one by one. This creates a linear history, with the rebased branch's commits appearing as if they were made directly on top of the target branch.

*Commit History:*
- Rebasing rewrites the commit history of the rebased branch, making it appear as if the commits were made directly on top of the target branch. It does not create merge commits.

Usage:

git checkout <branch_to_rebase>

git rebase <branch_to_rebase_onto>


*Commit History:*

- Merge preserves the commit history of both branches and explicitly indicates when and where branches were merged.
- Rebase creates a linear commit history by incorporating commits from one branch onto another without creating merge commits.

*Workflow:*

- Merge is a non-destructive operation that creates a merge commit, combining changes from different branches.
- Rebase is a more aggressive operation that rewrites commit history by applying commits from one branch on top of another, creating a linear history.


*Collaboration:*

- Merge is often used for integrating changes from feature branches into a main branch in collaborative environments.
- Rebase is useful for maintaining a clean and linear history, especially for feature branches, but it should be used with caution in shared repositories to avoid history rewriting conflicts.

  
*In summary, merge integrates changes by creating a merge commit, preserving branch history, while rebase integrates changes by rewriting commit history, creating a linear timeline. The choice between merge and rebase depends on project workflow, collaboration requirements, and preferences for commit history cleanliness.*
