# Git Commands Cheat Sheet

## Create a ssh key
Finds file in the whole filesystem

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

