# vscode-server-template
Run the full VSCode server within coder! (Enabled settings sync and Microsoft Marketplace)
**Thank you matifali#7055 for showing me that vscode-server exists!**

***Please note that this template uses software that is owned by Microsft. Please look at the licensing and terms [here](https://code.visualstudio.com/license/server)***

## Usage
Clone the repo and use the coder command to upload the template (*Make sure you have docker installed on the host!*)

```sh
git clone https://github.com/kozmiknano/vscode-server-template.git
cd vscode-server-template
coder template create
```

- The web client of vscode is on a subdomain rather than the traditional `/apps/code-server` Check out the terraform configuration for more info!

- I have made some branches with other forms of this template, such as slim; a completly bare bones environmnet with only the basic packages needed to run vscode-server.
    - You can view the list [here](https://github.com/KozmikNano/vscode-server-template/branches/all)
    - By clicking on one of the branches you can view more information about it.

## Notes
- This *should* work on any cpu arch.
- This template uses `ubuntu:latest` Docker
- NVM will be installed, alongside the latest node version, npm, yarn, and pnpm
- If in any case you are prompted for a password in the cli, you can use `password`

### Verified that it can run on arm based operating systems!
- I made/tested this on a Raspberry Pi 4B 8GB (ARM64 Raspberry Pi OS)
