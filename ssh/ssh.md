Check existing SSH keys:
```bash
ls -al ~/.ssh
```

Create SSH keys:
```bash 
ssh-keygen -t ed25519 -C "usermail@mail.com"
```

Run ssh-agent:
```bash
eval "$(ssh-agent -s)"
```
**Atention!** The ssh-agent is the program that will manage our SSH key. With the command below, we will initialize it and make it ready for the terminal to use to connect to the GitHub server. The message `Agent pid XXXXX` will be displayed indicating that the program was started successfully, with the number represented by `XXXXX` being a unique identifier.

Add the created key to ssh-agent:
```bash
ssh-add ~/.ssh/id_ed25519
```
**Atention!** If the key was created with a name other than the default, you must replace `id_ed25519` with it.

## References
[Connecting to GitHub with SSH](https://docs.github.com/en/authentication/connecting-to-github-with-ssh)