# Checkpoint2 Submission

** COURSE INFORMATION: CSN400NAA**

** STUDENT'S NAME: CHRISTO SHIBU KURIAN**

** STUDENT'S NUMBER: 147281208**

** GITHUB USER ID: 147281208-myseneca**

** TEACHER'S NAME: ATOOSA NASIRI**





### Table of Contents


1. [Part A - Adding Files - Local Repo Workflow](#header1)
   Refer to Checkpoint2/ folders

2. [Part B - Inspecting Local Repo with `git status` and `git log`](#header2)
  The key difference between the command 'git log' and 'git status' is its working area. git status pulls records from staging area and working directory whereas git log pulls the records only from the committed history.
  
  example: git log -n 5 will produce the last 5 commit logs. This output is shown under  PART C.
         git status: On branch CSN400
         Your branch is up to date with 'origin/CSN400'.

         Changes not staged for commit:
          (use "git add <file>..." to update what will be committed)
          (use "git restore <file>..." to discard changes in working directory)
               modified:   Checkpoint2/README.md

        no changes added to commit (use "git add" and/or "git commit -a")

3. [Part C - Creating & Merging Branches](#header3)
      $ git log -n 5
    commit 92748af3c1ca015a142c0fbc5502a600915a980f (HEAD -> CSN400, origin/HEAD, origin/CSN400)
    Author: cshibu-kurian <cshibu-kurian@myseneca.ca>
    Date:   Thu May 25 17:34:18 2023 -0400

        updating readme file with headers

    commit ac0214759ae93456f57ed7fa456c78ad18a3d9b3
    Author: cshibu-kurian <cshibu-kurian@myseneca.ca>
    Date:   Thu May 25 00:08:26 2023 -0400

        updated readme with answers

    commit 802ec1218f4cd3ab9bc3a50b22e0f33c3a9c336d
    Author: cshibu-kurian <cshibu-kurian@myseneca.ca>
    Date:   Thu May 25 00:04:53 2023 -0400

        Updating readme with answers

    commit 5701064abfcdac7345308966ac50bd9f560793aa (origin/feat-emojis, feat-emojis)
    Author: cshibu-kurian <cshibu-kurian@myseneca.ca>
    Date:   Wed May 24 23:26:04 2023 -0400

        adds emojis to feat-emojis branch

    commit 2d88464da22032bbecb7b1999267bc489b4e4000
    Author: cshibu-kurian <cshibu-kurian@myseneca.ca>
    Date:   Wed May 24 23:11:46 2023 -0400

        adds footnotes folder
    (END)
  

4. [Part D - Git Branching Strategy Review Question](#header4)

     ANSWERS
     1 . The 'main' is where the stable version of the code runs. Whereas the 'develop' branch runs parallel to the 'main' where multiple supporting branches branch out to test new code and released into the stable version.

    2.Release branch - where the already tested code in the 'develop' branch is ready to be merged into the 'main'.
   
      Feature branch - This branches out from the 'develop' but is never allowed to touch 'main'. This is where the experimental features' codes are scripted and tested.

      Hotfix branch - an emergency fix to the 'main' code created in the 'develop' and pushed quickly to 'main' before further data/information loss.


    3 i. Release branch must be publicly available to all devs.
      ii. Its always upto the Team Lead to merge the release code into 'main' branch with tag.




