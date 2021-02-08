# Setup git, Github and work with VSCode and PlatformIO

#### 1. Create Github account on github.com
#### 2. Accept the invitation of the T-systems-Youngsters admin
#### 3. Install git on you local computer. Use this link for Windows: https://git-scm.com/download/win just click through the installer.
#### 4. Open a commandline on Windows (win+r, type `cmd` enter).
Enter the following and replace the name and emailaddress:
```shell
git config --global user.name "$NAME"
git config --global user.email "$EMAIL"

```
#### 5. Generate an ssh-key by typing: `ssh-keygen` into the cmd and press enter several times to create a ssh-key.
#### 6. Open the file in `/Users/$USERNAME/.ssh/id_rsa.pub` with the windows editor and copy everything. 
#### 7. Go to github, click on you *account settings* -> *ssh and GPG keys*, *New SSH key* enter a name like *windows10* and paste the copied key beneath. Click *Add SSH key*. And may type your Github password afterwards.
#### 8. On Github click on the dropdown menu with your username on the left side and choose *T-systems-Youngsters* and then click the green *new* button.
#### 9. Enter the repository name. For us it's: `name-LOGIST` for Heiko it would be: `heiko-LOGIST`. Choose *public* and tick *Add a README file* and tick *Add .gitignore* -> choose C++ and click *create Repository*.
#### 10. On the following page click the green *code* button click on *ssh* and copy the link.
#### 11. Go back to the cmd and type `cd Documents` then `git clone $LINK` paste your copied link from Github and press enter to clone the repo. Type `yes` to confirm the hosts identity.
#### 12. Copy your `/Documents/Platformio/` directory into `/Documents/$USER-LOGIST` to track your code via git. When creating a new PlatformIO project, make sure to untick the *default location* and choose the cloned local copy of the git repository (`/Documents/$USER-LOGIST/Platformio/projects/`).
#### 13. Open VisualStudio Code Close all open VSC tabs and click on *File -> Open Folder* and choose your git repository (don't save workspace configuration). 
#### 14. Make changes to your files, for example: edit the README, create new directories, create new PlatformIO projects.
#### 15. Click on the branch symbol (Source COntrol) on the left side under the search icon and log VSC into your github account.
#### 16. After that you should see a number on the branch icon, this means there are untracked changes. Click on it and then click the `checkmark` icon (commit). Always stage changes. Provide a meaningfull commit message, this will be visible on github and should describe what you have changed. Note that you can only upload and compile when a PIO project is directly opened and not it's parent directories.
#### 17. Click on the three dots in the upper right corner next to the reload symbol and the *push* to upload your commits to github.
