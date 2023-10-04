# gcloud shortcuts
To setup and remember the commands

| Command | Description |
|---|---|
| project | Show current project |
| project-list | Show all projects with current loggedin account |
| project-change <projectID> | Change the current project |

## Setup
Add the aliasses of below to the ``.zshrc``

```
GCLOUD_SDK=$(which gcloud)
alias project='$GCLOUD_SDK config get-value project'
alias project-list='$GCLOUD_SDK projects list'
alias project-change='$GCLOUD_SDK config set project $@'
```
