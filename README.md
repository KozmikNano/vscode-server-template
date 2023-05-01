# Small Template
This version will only install the basic packages: ```sudo bash wget locales```

*Do to limitations of the `code tunnel` limitations alpine wasn't integrated. Ubuntu is still used as the base image.*

## vscode-server-template
Run the full VSCode server within coder! (Enabled settings sync and Microsoft Marketplace)
**Thank you matifali#7055 for showing me that vscode-server exists!**

***Please note that this template uses software that is owned by Microsft. Please look at the licensing and terms [here](https://code.visualstudio.com/license/server)***

### Usage
Clone the repo and use the coder command to upload the template (*Make sure you have docker installed on the host!*)

```sh
git clone https://github.com/kozmiknano/vscode-server-template.git
cd vscode-server-template
coder template create
```

### Notes
- This should work on any cpu arch.
- This template is on top of ubuntu (The latest)
- This template will install zsh using a tool from [this repo](https://github.com/deluan/zsh-in-docker)
    - Look at the dockerfile for more info
- NVM will be installed, alongside the latest node version

#### Verified that it can run on arm based operating systems!
- I made/tested this on a Raspberry Pi 4B 8GB (ARM64 Raspberry Pi OS)
