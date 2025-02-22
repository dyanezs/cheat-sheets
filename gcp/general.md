# General GCP Commands Cheat Sheet

## Set Account
When having more than one account, this command helps switching between them.

```bash
gcloud config set account "your-email@example.com"
```

You can check the changes with:

```
gcloud auth list
```

Also, before setting the project, it may ask you to login:

```
gcloud auth login
```

## Set Project
Same as accounts, you can switch between projects in the same account with this:

```bash
gcloud config set project <projet-id>
```

You can check changes with

```
gcloud config list
```

## Resource-Manager
I used this when I was trying to delete a project but got errors because previously I set some retention policies in GCS.

```bash
gcloud alpha resource-manager liens list --project <project-id>
```

The previous line triggered a package installation. After running successfully you get the corresponding ID

```bash
gcloud alpha resource-manager liens delete <name-of-lien>
```

Just after that, I was able to delete the project

```
gcloud projects delete <project-id>
```

## Delete Static IP Address
For some reason, in the Console, there's no option to delete these addresses when they have been released. I used this command in gcloud to delete them.

```bash
gcloud compute addresses delete <name-of-ip-address> --project <project-id> --region <region>
```
