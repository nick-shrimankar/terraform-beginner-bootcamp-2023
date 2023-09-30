# Terraform Beginner Bootcamp 2023

## Semantic Versioning!
This project uses semantic versioning for tagging.
[https://semver.org/](https://semver.org/)

Given a version number MAJOR.MINOR.PATCH, increment the:

- **MAJOR** version when you make incompatible API changes
- **MINOR** version when you add functionality in a backward compatible manner
- **PATCH** version when you make backward compatible bug fixes

Additional labels for pre-release and build metadata are available as extensions to the **MAJOR.MINOR.PATCH** format, ex: 1.0.1

## View your Linux OS type and version
### Consider checking your Linux distribution and change accordingly to distribution needs
- [Check Linux OS Type/Version](https://www.cyberciti.biz/faq/how-to-check-os-version-in-linux-command-line/)

Command -
```
$ cat /etc/os-release
```
Output -
```
PRETTY_NAME="Ubuntu 22.04.3 LTS"
NAME="Ubuntu"
VERSION_ID="22.04"
VERSION="22.04.3 LTS (Jammy Jellyfish)"
VERSION_CODENAME=jammy
ID=ubuntu
ID_LIKE=debian
HOME_URL="https://www.ubuntu.com/"
SUPPORT_URL="https://help.ubuntu.com/"
BUG_REPORT_URL="https://bugs.launchpad.net/ubuntu/"
PRIVACY_POLICY_URL="https://www.ubuntu.com/legal/terms-and-policies/privacy-policy"
UBUNTU_CODENAME=jammy
```
## Install the Terraform CLI
Initial TF installation instructions in gitpod.yml are outdated and has been changed.
### The Terraform CLI instructions are below -
[Install Terraform CLI](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli)

### sha-bang (#!)
https://en.wikipedia.org/wiki/Shebang_(Unix)

### chmod (_ch_ -ange _mod_ -e)
https://en.wikipedia.org/wiki/Chmod

### gitpod workspaces (before | init | command)
https://www.gitpod.io/docs/configure/workspaces/tasks

Init does not rerun if we restart an existing workspace.

### Created new bash script
Script created to support Terraform CLI installation. 
- All steps have ben added in bash script to keep it tidy
- Easy portability
- Easy to maintain for future updates

Terraform installation is multiple steps -
- created bin folder
- created bin/install_terraform_cli.sh
- chmod u+x ./bin/install_terraform_cli.sh

Updated gitpod.yml
- updated init to before (to ensure gitpod.yml works with gitpod)

