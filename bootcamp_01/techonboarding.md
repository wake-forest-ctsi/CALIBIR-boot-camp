# Getting Started

## Visual Studio Code

### Install VS Code

[Download from https://code.visualstudio.com/Download](https://code.visualstudio.com/Download) or run `winget install --id Microsoft.VisualStudioCode --source winget -ei`

Recommended Selections in installer:

- "Add Open with Code action to Windows Explorer file context menu"
- "Add Open with Code action to Windows Explorer directory context menu"

### Recommended Extensions

- [Python by Microsoft](https://marketplace.visualstudio.com/items?itemName=ms-python.python)
- [Docker by Microsoft](https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-docker)
- [Live Share by Microsoft](https://marketplace.visualstudio.com/items?itemName=MS-vsliveshare.vsliveshare)
- [GitHub Theme by GitHub](https://marketplace.visualstudio.com/items?itemName=GitHub.github-vscode-theme)
- [Markdown All in One by Yu Zhang](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one)
- [indent-rainbow by oderwat](https://marketplace.visualstudio.com/items?itemName=oderwat.indent-rainbow)
- 

## Git / GitHub

### How to Install Git

[Download from https://git-scm.com/downloads](https://github.com/git-for-windows/git/releases/download/v2.40.1.windows.1/Git-2.40.1-64-bit.exe) or run `winget install --id Git.Git --source winget -ei`

Recommended Selections in installer:

- "Use Visual Studio Code as Git's default editor"
- "Override the default branch name for new repositories" - main
- "use external OpenSSH"
- "use the native Windows Secure Channel library" - THIS IS IMPORTANT

### How to Clone this repo

```
git clone https://github.com/wake-forest-ctsi/CALIBIR-boot-camp.git .
```

[backup plan](https://github.com/wake-forest-ctsi/CALIBIR-boot-camp/archive/refs/heads/main.zip)

### Things to know about Git

Basic Configuration (needed before commit):

```shell
git config --global credential.helper store
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
```

To update from Command Prompt `git update-git-for-windows`

## Docker

### Useful commands to know

These are useful if you JupyterLab instance has locked up

* `docker ps` list running containers
* `docker kill $(docker ps -q)` stop any running containers
* `docker rm $(docker ps -aq)` remove any stopped containers
* `docker logs wfbmi-dev` If you need to get the url\token to log back into your instance

## Jupyter

See [Notebook](JupyterIntro.ipynb)

### To Spin up Jupter Lab locally

```shell
docker run -p 8888:8888 -v C:/home:/home/jovyan/work --user root -e JUPYTER_ENABLE_LAB=yes -e GRANT_SUDO=yes --name wfbmi-dev ghcr.io/wake-forest-ctsi/wfbmi-dev:latest
```
*Note:* I've recently updated the image source from `jupyter/datascience-notebook:latest` to bake in some customizations.  Please use the updated version above if you have any certificate issues.

### If you lose/forget your token

- Start up the wfbmi-dev container in docker desktop
- click on logs and look for the login url
- if you can't find it there, open up command prompt and run the following:
  ```shell
    docker exec wfbmi-dev jupyter server list
  ```
*Note:* The url in this output will give you security errors.  Please use `http://localhost:8888/?token=` instead.
## VPN Access

- [Request VPN access for your userID](https://wakehealth.service-now.com/sp?id=sc_cat_item&sys_id=381615be37b00a80c113a9c2b3990e1c&sysparm_category=c23325bc37b88680c113a9c2b3990e16)
- [Videos to setup RSA app on your phone](https://www.wakehealth.edu/About-Us/Our-Website/ITS)
- [RSA portal to associate phone](https://wakehealth.auth.securid.com/mypage)
- The app you need to install is called RSA SecurID Authenticate

## MatLab license request

https://www.mathworks.com/academia/tah-portal/wake-forest-university-40638205.html

## CITI Training

Before being able to access PHI, you must complete ​[CITI training](https://about.citiprogram.org/en/homepage/) (and do so every three years). The relevant course is called Biomedical Investigators (Human Research > Biomedical Investigators > Basic Course).

The first time you do this it will likely take you a couple of hours. Make sure you associate your account/certification with Wake Forest School of Medicine (ID: 438)


