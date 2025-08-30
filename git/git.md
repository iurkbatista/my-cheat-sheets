Install git:
```bash
sudo apt install git
```

Check the installed version:
```bash
git --version
```

Check the settings for git:
```bash
git config --list
```

Configure user and email for git:
```bash
git config --global user.name = "User Name"
git config --global user.email = "usermail@mail.com"
```

Configure the code editor for git:
```bash
git config --global core.editor "code --wait"
```
**Attention!** When we run a git command that requires a code editor, for example, to write a commit message, git opens the configured editor, in this case VScode. The `--wait` flag tells git to wait until you save and/or close the file in VScode, ensuring that your edit is complete before the git process continues. Without this flag, the editor would open and close immediately.

Set the default name for the initial branch:
```bash
git config --global init.defaultBranch main
```

Start a new git repository in a local folder:
```bash
git init
```

Adds modified and new files to the current directory and subfolders:
```bash
git add .
```

Adds all modified, new, and deleted files to the entire repository:
```bash
git add -A
```

List remote origin:
```bash
git remot -V
```

Remove remote origin:
```bash
git remote remove origin
```

Set the repository url:
```bash
#For HTTP
git remote set-url origin https://github.com/user-name/repository.git

#For SSH
git remote set-url origin git@github.com:user-name/repository.git
```