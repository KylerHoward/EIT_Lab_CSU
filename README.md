# EIT_Lab_CSU
Collection of presentations and documents from the EIT lab at CSU


# Documentation/Tutorial

* [Git Documentation](https://git-scm.com/doc)
* [Links to various Git trainings](https://git-scm.com/doc/ext)
  * Suggest [Git Beginners Guide for Dummies](https://git-scm.com/doc/ext) as as a good starting point

## Commands to run 
Installing git to your Windows device

**Step 1:** Open powershell and install chocolatey

Run powershell with admin. If it prompts you if you want to continue, say "Y"

    Set-ExecutionPolicy AllSigned

    Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
    
    choco install git
    
**Step 2:** Close Powershell window

**Step 3:** Install the git repository where you want it

Open new powershell window

Navigate to where you want the code to be stored. If you have spaces in folder names, you need "" around the address. If there are no spaces, "" are not needed

    cd "folder address"
    (ex: cd "C:\Users\kyler\OneDrive\School\Colorado State\Research\Dr. Mueller")
    (ex: cd C:\Users\kyler\OneDrive\School\Colorado_State\Research\Dr._Mueller)
    
    git clone https://github.com/KylerHoward/EIT_Lab_CSU.git


## To do work
**Step 1:** Setting up workspace

Open up powershell and navigate to the repository that you are working on

    cd "file address" 
    (ex: C:\Users\kyler\OneDrive\School\Colorado State\Research\Dr. Mueller\EIT_Lab_CSU")

To pull in latest code (updating your side of things)

    git pull 

To see what files are in the current branch

    ls

To make a new branch to work in

    git checkout -b "name of branch (YourName-branch-name)"
    (ex: git checkout -b KylerHoward-upload-presentation)
    
**Step 2:** Working on the code

Open and edit the files like you normaly would. You can minimize powershell while editing files

Once done, it is good to check what changes have been made

    git status
    
To add your files so they will be updated

    git add "file name"
    
To save your changes

    git commit -m "description of edits"
    
**Step 3:** Updating your code to the shared repository 

To send changes to git hub server. This might pull up a line of command that you need to copy and paste

    git push

Go to main git hub repository website to make pull request (https://github.com/KylerHoward/EIT_Lab_CSU.git)

Make a pull request to sync your code to the repository. Someone will hopefully approve it, squash and merge to master, and delete the branch

Go back to the master branch to start again

    git checkout master

Start from top again or close powershell
