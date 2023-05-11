# Biomedical Informatics Bootcamp

## Schedule

- [Informatics Bootcamp 1: Healthcare Informatics / May 30th 1:00 pm - 2:00 pm](./bootcamp_01/agenda.md)
- [Informatics Bootcamp 2: Imaging Informatics / May 31st 1:00 pm - 2:30 pm](./bootcamp_02/agenda.md)
- [Informatics Bootcamp 3: Clinical Informatics / June 1st 1:00 pm - 2:30 pm](./bootcamp_03/agenda.md)
- [Informatics Bootcamp 4: Translational Bioinformatics / June 2nd 1:30 pm - 3:00 pm](./bootcamp_04/agenda.md)
- [Informatics Bootcamp 5: Artificial Intelligence / June 5th 1:00 pm - 2:30 pm](./bootcamp_05/agenda.md)

## Default Docker container

docker run -p 8888:8888 -v c:/opt/docker/work:/home/jovyan/work --user root -e JUPYTER_ENABLE_LAB=yes -e GRANT_SUDO=yes --name wfbmi-dev jupyter/datascience-notebook:latest
