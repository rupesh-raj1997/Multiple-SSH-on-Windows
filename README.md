# Multiple-SSH-on-Windows

# Setup Multiple SSH Keys on Windows 10

As suggested in the title, folks who want to work with multiple SSH keys can follow this README.

## Creating Keys

Use [this](https://www.domstamand.com/managing-multiple-ssh-keys-for-authentication-to-github-on-windows-10/) to create multiple SSH keys on windows.

### Cloning the Repository
This one is fairly evident but make sure you use the ssh link on GitHub while cloning locally.

### Updating Config
This one is important, you first need to run the following commands to update your git config file. Refer to [this](https://gist.github.com/jexchan/2351996) for step by step.

```
$ git config user.name "jexchan"
$ git config user.email "jexchan@gmail.com" 

```
Next you update the remote ref at `.git/config` manually, This works like creating an alias
```
[remote "origin"]
        url = git@github.com-work:ORGANIZATION/gfs.git
```
