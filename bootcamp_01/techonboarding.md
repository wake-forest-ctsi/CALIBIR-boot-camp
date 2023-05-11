# Getting Started

## Git

TO COME

To setup git (needed before commit):
```shell
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
git config --global credential.helper store
```

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
docker run -p 8888:8888 -v C:\home:/home/jovyan/work --user root -e JUPYTER_ENABLE_LAB=yes -e GRANT_SUDO=yes --name wfbmi-dev jupyter/datascience-notebook:latest
```


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


