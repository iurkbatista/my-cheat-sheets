View the contents of your public [SSH key](../ssh/ssh.md) and add it to your GitHub settings:
```bash
cat ~/.ssh/id_ed25519.pub
```

Test your SSH connection:
```bash
ssh -T git@github.com
```