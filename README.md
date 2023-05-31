# Biomedical Informatics Bootcamp

## Schedule

- [Informatics Bootcamp 1: Healthcare Informatics / May 30th 1:00 pm - 2:30 pm](./bootcamp_01/agenda.md)
- [Informatics Bootcamp 2: Imaging Informatics / May 31st 1:00 pm - 2:30 pm](./bootcamp_02/agenda.md)
- [Informatics Bootcamp 3: Clinical Informatics / June 1st 1:00 pm - 2:30 pm](./bootcamp_03/agenda.md)
- [Informatics Bootcamp 4: Translational Bioinformatics / June 2nd 1:30 pm - 3:00 pm](./bootcamp_04/agenda.md)
- [Informatics Bootcamp 5: Artificial Intelligence / June 5th 1:00 pm - 2:30 pm](./bootcamp_05/agenda.md)

## Default Docker container

```shell
docker run -p 8888:8888 -v C:/home:/home/jovyan/work --user root -e JUPYTER_ENABLE_LAB=yes -e GRANT_SUDO=yes --name wfbmi-dev ghcr.io/wake-forest-ctsi/wfbmi-dev:latest
```
*Note:* I've recently updated the image source from `jupyter/datascience-notebook:latest` to bake in some customizations.  Please use the updated version above if you have any certificate issues.
