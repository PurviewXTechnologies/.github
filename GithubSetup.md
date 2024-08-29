# Git Installation and Configuration Guide

This guide provides step-by-step instructions for installing Git, generating an SSH key, and configuring Git on your system.

## Step 1: Install Git

### Windows
1. Download Git for Windows from [git-scm.com](https://git-scm.com/download/win).
2. Run the installer and follow the default installation steps.

### macOS
1. Install Git using Homebrew:
   ```bash
   brew install git
   ```

## Step 2: Generate an SSH Key
1. Open a terminal or Git Bash.
2. Run the following command to generate an SSH key using the ed25519 algorithm:
   ```bash
    ssh-keygen -t ed25519 -C "gitpurviewdevs@gmail.com"

3. Press Enter to save the key in the default location (~/.ssh/id_ed25519).
4. Optionally, enter a passphrase for added security or press Enter to skip.

## Step 3: Configure Git
### Set your Git username:
    ```bash
        git config --global user.name "DevPurview"
    ```    
### Set your Git email:
    ```bash
        git config --global user.email "gitpurviewdevs@gmail.com"
    ```
## Step 4: Copy the SSH Key to Your Clipboard
### Linux/macOS:
    ```bash
        cat ~/.ssh/id_ed25519.pub | pbcopy
    ```    
### Windows (Git Bash):
    ```bash
        clip < ~/.ssh/id_ed25519.pub
    ```    

## Step 5: Now press Windows + V in user's system
- Now copy the ssh value 

## Step 6: Add the SSH Value to Your GitHub Account (Admin Account)
1. Log in to your GitHub account.
2. Go to your profile icon in the top right corner and select Settings.
3. In the left sidebar, click on SSH and GPG keys.
4. Click the New SSH key button.
   - In the "Title" field, enter a descriptive name for the key (e.g., "My Laptop SSH Key").
   - Paste the SSH Value you copied earlier into the "Key" field.
5. Click on the Add SSH key button to save.