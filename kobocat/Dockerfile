FROM kobotoolbox/kobocat:2.019.22

COPY ./files/scripts/wait_for_mongo.bash /etc/my_init.d/01_wait_for_mongo.bash
COPY ./files/scripts/wait_for_postgres.bash /etc/my_init.d/02_wait_for_postgres.bash
COPY ./files/scripts/wait_for_kpi.bash /etc/my_init.d/03_wait_for_kpi.bash
COPY ./files/scripts/runtime_variables_kobocat.source.bash /etc/profile.d/runtime_variables_kobocat.source.bash.sh
COPY ./files/uwsgi/kc_uwsgi.ini /srv/src/kobocat/docker/kobocat.ini
