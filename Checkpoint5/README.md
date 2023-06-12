# Checkpoint5 Submission

- **COURSE INFORMATION: CSN400NAA**

- **STUDENT’S NAME: CHRISTO SHIBU KURIAN**

- **STUDENT'S NUMBER: 147281208**

- **GITHUB USER ID: 147281208-myseneca**

- **TEACHER’S NAME: ATOOSA NASIRI**



### Table of Contents

1. [Part A - Containerize an application]
  
     Answer 1 : 

         This can be due to variety of reasons, mainly due to caching mechanisms, changes in the build context, modifications in the Dockerfile, dependencies and external resources, and even parallel builds.

     Answer 2 :
 
        The '-t' flag is assigned to specify the tag for the image

       CSK@CSK-hp MINGW64 ~/Documents/Backup/CSN400AA/getting-started/app (master)
       $ docker build getting-started .
         ERROR: "docker buildx build" requires exactly 1 argument.
         See 'docker buildx build --help'.

         Usage:  docker buildx build [OPTIONS] PATH | URL | -

         Start a build

     
     Answer 3 :

         Each time the build process produces the same image, such as the same layers and their content, Docker automatically identifies the redundancy and avoids creating duplicate images. 
     
     
     Answer 4 :
               CSK@CSK-hp MINGW64 ~/Documents/Backup/CSN400AA/getting-started/app (master)
               $ docker run -p 1000:3000 getting-started
                 Using sqlite database at /etc/todos/todo.db
                 Listening on port 3000


     Answer 5 :    port 3000
     
     
     Answer 6 :
        
          CSK@CSK-hp MINGW64 ~/Documents/Backup/CSN400AA/getting-started/app (master)
          $ docker ps
            CONTAINER ID   IMAGE             COMMAND                  CREATED          STATUS          PORTS                    NAMES
            78cc0f841874   getting-started   "docker-entrypoint.s…"   16 minutes ago   Up 16 minutes   0.0.0.0:3000->3000/tcp   dazzling_elbakyan


     
     
     Answer 7 : the time is longer
      
     Answer 8 : 
       
        docker: Error response from daemon: driver failed programming external connectivity on endpoint laughing_burnell 
                 (bb242b2ca4d67eba76e79474fb36bb5125708ebdabd7f45c8eaf16caaabde9dd): Bind for 0.0.0.0:3000 failed: port is already allocated.

     
     
     Answer 9 : 
        ![](Screenshot%20(261).png)




2. [Part B - Share the application]
         ![](Screenshot%20(259).png)
         ![](Screenshot%20(260).png)    


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

    output of SHOW DATABASES;
         
         Copyright (c) 2000, 2023, Oracle and/or its affiliates.

         Oracle is a registered trademark of Oracle Corporation and/or it s
         affiliates. Other names may be trademarks of their respective
         owners.

         Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

         mysql> SHOW DATABASES;
         +--------------------+
         | Database           |
         +--------------------+
         | information_schema |
         | mysql              |
         | performance_schema |
         | sys                |
         | todos              |
         +--------------------+
         5 rows in set (0.00 sec)


     output of $ dig mysql

        6f7f7caf080c  ~  dig mysql

        ; <<>> DiG 9.18.13 <<>> mysql
        ;; global options: +cmd
        ;; Got answer:
        ;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 12337 
        ;; flags: qr rd ra; QUERY: 1, ANSWER: 1, AUTHORITY: 0, ADDITIONAL: 0

        ;; QUESTION SECTION:
        ;mysql.                         IN      A

        ;; ANSWER SECTION:
        mysql.                  600     IN      A       172.18.0.2

        ;; Query time: 0 msec
        ;; SERVER: 127.0.0.11#53(127.0.0.11) (UDP) 
        ;; WHEN: Sun Jun 11 22:58:32 UTC 2023
        ;; MSG SIZE  rcvd: 44


