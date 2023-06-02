# Checkpoint3 Submission

- **COURSE INFORMATION: CSN400NAA**
 
- **STUDENT’S NAME: Christo Shibu Kurian**

- **STUDENT'S NUMBER: 147281208**

- **GITHUB USER ID: 147281208-myseneca**

- **TEACHER’S NAME: Atoosa Nasiri**


### Table of Contents

1. [Part A - Manage Conflicts - Overwrite Remote Changes]
 
     Below is the log file of conflict error-

   
    Pushing to https://github.com/147281208-myseneca/CSN400-Capstone.git
 To https://github.com/147281208-myseneca/CSN400-Capstone.git
  ! [rejected]        CSN400 -> CSN400 (fetch first)
 error: failed to push some refs to 'https://github.com/147281208-myseneca/CSN400-Capstone.git'
 hint: Updates were rejected because the remote contains work that you do
 hint: not have locally. This is usually caused by another repository pushing
 hint: to the same ref. You may want to first integrate the remote changes
 hint: (e.g., 'git pull ...') before pushing again.
 hint: See the 'Note about fast-forwards' in 'git push --help' for details.



    Below is the log file of overwrite


   POST git-receive-pack (9053 bytes)
remote: Resolving deltas:   0% (0/10)        
remote: Resolving deltas:  10% (1/10)        
remote: Resolving deltas:  20% (2/10)        
remote: Resolving deltas:  30% (3/10)        
remote: Resolving deltas:  40% (4/10)        
remote: Resolving deltas:  50% (5/10)        
remote: Resolving deltas:  60% (6/10)        
remote: Resolving deltas:  70% (7/10)        
remote: Resolving deltas:  80% (8/10)        
remote: Resolving deltas:  90% (9/10)        
remote: Resolving deltas: 100% (10/10)        
remote: Resolving deltas: 100% (10/10), completed with 1 local object.        
Pushing to https://github.com/147281208-myseneca/CSN400-Capstone.git
   To https://github.com/147281208-myseneca/CSN400-Capstone.git
    + c3cab25...afaa217 CSN400 -> CSN400 (forced update)
       updating local tracking ref 'refs/remotes/origin/CSN400'


       After pushing the local changes to remote, the color of text is changed to 'green'
  


2. [Part B - Manage Conflicts - Reset Local Commit Head]

      Below is the log of pull error 

      Pushing to https://github.com/147281208-myseneca/CSN400-Capstone.git
To https://github.com/147281208-myseneca/CSN400-Capstone.git
 ! [rejected]        CSN400 -> CSN400 (fetch first)
error: failed to push some refs to 'https://github.com/147281208-myseneca/CSN400-Capstone.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.


      Below is the log of head reset

    HEAD is now at afaa217 first attempt to push index.html
 commit afaa2177c90ac0db79927add220d766e798f81d1
 Author: cshibu-kurian <cshibu-kurian@myseneca.ca>
 Date:   Thu Jun 1 03:46:30 2023 -0400

    first attempt to push index.html


    Below is the log of pull success

    POST git-upload-pack (198 bytes)
 From https://github.com/147281208-myseneca/CSN400-Capstone
 = [up to date]      CSN400      -> origin/CSN400
 = [up to date]      OPS445      -> origin/OPS445
 = [up to date]      feat-emojis -> origin/feat-emojis
 Updating afaa217..f1dd358
 Fast-forward
  Checkpoint3/conflict-resolution/index.html | 2 +-
  1 file changed, 1 insertion(+), 1 deletion(-)


      After pushing the local changes to remote, the color of text is changed to 'darkolivegreen'



3. [Part C - Manage Conflicts - Merge Editor]

   Below is the log of pull conflict
      

      POST git-upload-pack (375 bytes)
     From https://github.com/147281208-myseneca/CSN400-Capstone
      * branch            feat-body-text -> FETCH_HEAD
      = [up to date]      feat-body-text -> origin/feat-body-text
     Already up to date.


     Below is the status log

     On branch master

     No commits yet

     Untracked files:
       (use "git add <file>..." to include in what will be committed)
	   ../../../../.bash_history
	   ../../../../.gitconfig
	   ../../../../.lesshst
	   ../../../../.packettracer
	   ../../../../.ssh/
	   ../../../../.vscode/
	   ../../../../3D Objects/
	   ../../../../AppData/
	   ../../../../CSN400-Capstone/
	   ../../../../Checkpoint1/
	   ../../../../Cisco Packet Tracer 8.2.0/
	   ../../../../Cisco Packet Tracer 8.2.1/
	   ../../../../Contacts/
	   ../../../../Desktop/
	   ../../../
	   ../../../../Downloads/
	   ../../../../Favorites/
	   ../../../../Links/
	   ../../../../Music/
	   ../../../../NTUSER.DAT
	   ../../../../NTUSER.DAT{4d95c0bf-72af-11ed-8850-a840c853de45}.TM.blf
	   ../../../../NTUSER.DAT{4d95c0bf-72af-11ed-8850-a840c853de45}.TMContainer00000000000000000001.regtrans-ms
	   ../../../../NTUSER.DAT{4d95c0bf-72af-11ed-8850-a840c853de45}.TMContainer00000000000000000002.regtrans-ms
	   ../../../../OneDrive/
	   ../../../../Pictures/
	   ../../../../Saved Games/
	   ../../../../Searches/
	   ../../../../Videos/
	   ../../../../ex-list
	   ../../../../ntuser.dat.LOG1
	   ../../../../ntuser.dat.LOG2
	   ../../../../ntuser.ini

     nothing added to commit but untracked files present (use "git add" to track)



       Screenshot of the remote script Screesnot (234)

  

4. [Part D - Collaboration - Creating Pull Request]

       Screeshot of pull request added  Screenshot (233)
