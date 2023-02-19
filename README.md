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
* install the required version node
```
nvm alias default "version of node"
```
* install the latest version npm with nvm
```
nvm install-latest-npm
```
