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


## Deploy Notes

Need to update the static locations in the `etc/nginx/sites-enabled/default` file;

Make the following changes;

   - `/var/www/kobocat` ->` `/var/www`
   - `/var/www/kpi` -> `/var/www`

Due to the limitations of the volume mount. Ideally it would be better to have separate volume mounts for these 2 directories, to prevent potential clashes.
