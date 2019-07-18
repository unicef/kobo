# UNICEF Kobo Containers

Dockerfiles and scripts that allow the relevant containers to be built in order to run Kobo in rancher.
Based off of https://github.com/kobotoolbox/kobo-docker

## Build Containers

For each container;

    - enketo_express
    - kobocat
    - kpi
    - nginx

You can build with;

    docker build -t <tag> .


And then push with;

    docker push <tag>
