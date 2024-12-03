# dont-you-love-banners [300]
---
![image](https://github.com/HAW-THL/Write-ups/assets/90260119/7ce9fdda-eb17-48bc-a8cb-f1335fca8011)

- Log into the first Server with NetCat
```
nc tethys.picoctf.net 61371
```
![image](https://github.com/HAW-THL/Write-ups/assets/90260119/9b740f26-350d-47a7-9249-c846b9076bd2)

- Here we see two things: the SSH version and something that points to a password that we need for the next server

- Now we log into the second server
```
nc tethys.picoctf.net 58476
```
![image](https://github.com/HAW-THL/Write-ups/assets/90260119/cd451afd-1c8d-44bc-ad94-5a5e365bded3)

- Here we answer the questions and are in the shell

![image](https://github.com/HAW-THL/Write-ups/assets/90260119/175214fd-d64b-46c8-9993-2ec25cc0764c)

- First we look with "ls" and see "banner" which is the banner from the beginning and "text" which says "keep digging"
- Then we look in the parent directory
- After a bit of digging we find the root directory, in which we find two files "flag.txt" and "script.py"

![image](https://github.com/HAW-THL/Write-ups/assets/90260119/2d0c4ead-89ea-4c55-a80a-366b95a7b434)

- Unfortunately we cannot read the “flag.txt” but “script.py” executes the same program as when you connect to the server
- The banner is the same as in the “player” directory

![image](https://github.com/HAW-THL/Write-ups/assets/90260119/f883b697-49da-4c8e-b196-24deefdd8dc7)

- Now we can go back to the "player" directory and delete the original banner
- Then we create a [Symlink](https://en.wikipedia.org/wiki/Symbolic_link) from the flag in the "player" directory, which we call "banner"
```
ln -s /root/flag.txt banner
```
> This command creates a symbolic link called "banner" in the current directory that points to the file "/root/flag.txt". Symbolic links are links to files or directories that refer to other files or directories. In this case, the symbolic link "banner" would point to the file "/root/flag.txt"

- Now we can reconnect to the server so that when we connect to the server, we read the flag rather than the actual banner

![image](https://github.com/HAW-THL/Write-ups/assets/90260119/3648bf51-1c7c-4914-8e60-a7138843cfc8)

```
picoCTF{b4nn3r_gr4bb1n9_su((3sfu11y_218ef5d6}
```
