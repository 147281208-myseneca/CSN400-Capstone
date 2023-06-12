# Checkpoint5 Submission

- **COURSE INFORMATION: CSN400NAA**

- **STUDENT’S NAME: CHRISTO SHIBU KURIAN**

- **STUDENT'S NUMBER: 147281208**

- **GITHUB USER ID: 147281208-myseneca**

- **TEACHER’S NAME: ATOOSA NASIRI**



### Table of Contents

1. [Part A - Containerize an application]
  
     Answer 1 : 

     Answer 2 :
 
        The '-t' flag is assigned to specify the tag for the image

       CSK@CSK-hp MINGW64 ~/Documents/Backup/CSN400AA/getting-started/app (master)
       $ docker build getting-started .
         ERROR: "docker buildx build" requires exactly 1 argument.
         See 'docker buildx build --help'.

         Usage:  docker buildx build [OPTIONS] PATH | URL | -

         Start a build

     
     Answer 3 :
     
     
     Answer 4 :
               CSK@CSK-hp MINGW64 ~/Documents/Backup/CSN400AA/getting-started/app (master)
               $ docker run -p 1000:3000 getting-started
                 Using sqlite database at /etc/todos/todo.db
                 Listening on port 3000


     Answer 5 :
     
     
     Answer 6 :
        
          CSK@CSK-hp MINGW64 ~/Documents/Backup/CSN400AA/getting-started/app (master)
          $ docker ps
            CONTAINER ID   IMAGE             COMMAND                  CREATED          STATUS          PORTS                    NAMES
            78cc0f841874   getting-started   "docker-entrypoint.s…"   16 minutes ago   Up 16 minutes   0.0.0.0:3000->3000/tcp   dazzling_elbakyan


     
     
     Answer 7 :
      
     Answer 8 : 
       
        docker: Error response from daemon: driver failed programming external connectivity on endpoint laughing_burnell 
                 (bb242b2ca4d67eba76e79474fb36bb5125708ebdabd7f45c8eaf16caaabde9dd): Bind for 0.0.0.0:3000 failed: port is already allocated.

     
     
     Answer 9 :
2. [Part B - Share the application]

3. [Part C - Persist the DB]


       CSK@CSK-hp MINGW64 ~/Documents/Backup/CSN400AA/getting-started/app (master)
       $ docker volume inspect todo-db
        [
           {
                "CreatedAt": "2023-06-11T21:18:45Z",
                "Driver": "local",
                "Labels": null,
                "Mountpoint": "/var/lib/docker/volumes/todo-db/_data",
                "Name": "todo-db",
                "Options": null,
                "Scope": "local"
            }
        ]



4. [Part D - Multi container apps]