# Git Commands Cheat Sheet

## Create a SSH Key
Create ssh key

```bash
ssh-keygen -t rsa -b 4096 -C "your-email@example.com"
```

- You'll be prompted to enter the file in which to save the key. By default, it will suggest the path `~/.ssh/id_rsa`.
- You can define a passphrase.

After this
```bash
ssh-add ~/.ssh/id_rsa
```

- Then copy the contents of the public key `~/.ssh/id_rsa.pub` and add it to your GitHub account.
- Visit your GitHub SSH and GPG keys settings.
- Click on "New SSH key" or "Add SSH key."
- Paste the key into the "Key" field.

## Pull from Remote Branch
Assuming, we've already cloned the repo with master/main branch in our local, and now we want to pull a specific branch `development`.
```bash
git pull origin development
```
