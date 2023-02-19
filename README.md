# nvm-Install-Guide
> Node Version Manager (nvm) - detailed guide for correct installation and configuration.

1. If you do not have Git, then you need to install it using the link: https://git-scm.com/downloads

2. After installation, open git-bash and install nvm in one of two ways:
```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
```
```
wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
```
3. Then enter the following command in the terminal:
```
export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"
```
4. Node Version Manager is now installed and we will check it with the command showing the current nvm version:
```
nvm -v
```
> Here is a list of commands for fast and comfortable work with nvm:
* install the latest version node:
```
nvm install node
```
* install the required version node:
```
nvm install 10.14.0
```
* set the required version by default:
```
nvm alias default "version of node"
```
* install the latest version npm with nvm:
```
nvm install-latest-npm
```
* list of installed version node:
```
nvm ls
```
# Fix errors
> If you have not saved any changes after closing git-bash, then you need to manually make changes to the <code>.bash_profile</code> file (it may be called differently depending on the operating system)

Open this file and add the following lines to the end of it:
```
export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"
```
After adding them, further changes to nvm in git-bash will be saved.
