## Lab 02

- Name:anuja alluri
- Email: alluri.17@wright.edu

## Part 1 Answers

The answers for this section are to help you record what steps  
are needed to create a file locally (in your cloned repo)  
and push them (sync) with GitHub

1. Add a file for tracking:git add file_name
2. Commit changes: git commit
3. Sync local commits with GitHub:git push

## Part 2 Answers

For each, write the command used or answer the question posed.

1.sudo adduser bob
2./home/bob
3.no because i dont have any permissions
4.su bob
5.cd ~
6. bob is the  owner he has permissions to add files to his directory.
7.exit
8.cd

## Part 3 Answers

For each, write the command used or answer the question posed.

1.sudo groupadd crew
2.sudo usermod -aG crew bob
3.sudo chgrp crew DirA
4.su bob 
5.touch "file.txt"
6.Because bob is a part of crew group which has permissions to DirA

## Part 4 Answers

For each, write the command used or answer the question posed.

1.sudo touch sudowho.txt
2.-rw-r--r--
3.vim sudowho.txt
add text then ":wq!" to overwrite and save

## Part 5 Answers

1. `ssh` command before configuring `config` file: ssh -i ceg.pem ubuntu@52.87.136.118
2. HostName:52.87.136.118
3. User:ubuntu
4. IdentityFile:/Users/raj/ceg.pem
5. `~/.ssh/config` contents:

```
Host anu
    HostName 52.87.136.118
    User ubuntu
    IdentityFile /Users/raj/ceg.pem
```

6. `ssh` command after configuring `config` file: ssh anu
