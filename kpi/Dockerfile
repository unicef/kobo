FROM kobotoolbox/kpi:2.019.23

COPY ./files/scripts/wait_for_mongo.bash /etc/my_init.d/01_wait_for_mongo.bash
COPY ./files/scripts/wait_for_postgres.bash /etc/my_init.d/02_wait_for_postgres.bash
COPY ./files/scripts/create_kobo_superuser.bash /etc/my_init.d/20_create_kobo_superuser.bash
COPY ./files/scripts/runtime_variables_kpi.source.bash /etc/profile.d/runtime_variables_kpi.source.bash.sh
COPY ./files/uwsgi/kpi_uwsgi.ini /srv/src/kpi/uwsgi.ini
