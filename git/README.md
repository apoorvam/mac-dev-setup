# Git

Git is a version-control system for tracking changes in computer files and coordinating work on those files among multiple people.

## Installation
	
```
$ brew install git
```

To set username and email to be used for your Git commits globally, you can run following commands:
```
$ git config --global user.name "Your Name Here"
$ git config --global user.email "your_email@youremail.com"
```

## Generating a new SSH key

Run below command to create a new ssh key, using the provided email as a label. This generates a public/private rsa key pair.
```
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```

When you're prompted to "Enter a file in which to save the key," press Enter. This accepts the default file location. You can also set a passphrase if required, else you can just press Enter.

## Adding your SSH key to the ssh-agent

Start the ssh-agent in the background.

```
$ eval "$(ssh-agent -s)"
Agent pid 59566
```
If you're using macOS Sierra 10.12.2 or later, you will need to modify your ~/.ssh/config file to automatically load keys into the ssh-agent and store passphrases in your keychain.

```
Host *
 AddKeysToAgent yes
 UseKeychain yes
 IdentityFile ~/.ssh/id_rsa
```
Add your SSH private key to the ssh-agent and store your passphrase in the keychain. If you created your key with a different name, or if you are adding an existing key that has a different name, replace id_rsa in the command with the name of your private key file.

```
ssh-add -K ~/.ssh/id_rsa
```

## Add SSH key to Github account

Copy your SSH key by issuing command:
```
$ pbcopy < ~/.ssh/id_rsa.pub
```
Paste it under Profile Settings of Github -> SSH Keys

This enables you to use SSH for pushing your commits instead of https, after updating your remote url.