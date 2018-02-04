## Bash Ubuntu on Windows 10

NOTE: Some of these commands won't give you visual feedback.

1. Install ms vscode

2. Windows search and enable "developer mode"

3. Open Control Panel > Programs > Turn Windows features on or off > Windows Subsystem for Linux

4. Open Microsoft Store

5. Get/Install Ubuntu  (this may take some time, terminal window should open automatically when finished)

6. Create a username (your first name) and password 

7. type ```ls -a``` and you should see .bashrc file

9. type ```echo "cd /mnt/c/Users/$USER" >> .bash_profile``` and this will make it so bash launches in your windows home directory

10. type ```cat .bashrc``` to see it print what you did in step 9

11. type ```sudo apt-get update -y``` and install (this may take some time)

12. type ```sudo apt-get upgrade -y``` and install (this may take some time)

13. type ```sudo apt-get dist-upgrade -y``` and isntall (this may take some time)

14. At this point it's a good idea to pin bash to your windows taskbar, close bash and open it again

15. type ```pwd``` and it should print out your windows home directory (Documents, Pictures etc) 

16. type ```mkdir apps``` to create a folder for keeping apps

17. Open vs code

18. File > Preferences > Settings

19. Right hand side in custom settings copy and paste the code below after a comma.
```
"terminal.external.windowsExec": "C:\\Windows\\System32\\bash.exe",
"terminal.integrated.shell.windows": "C:\\Windows\\System32\\bash.exe",
```

20. Quit vs code and reopen - now the integrated terminal will have bash

21. Install git, rbenv and ruby (instructions in other resources) using bash