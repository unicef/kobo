FROM kobotoolbox/enketo-express-extra-widgets:1.77.0-jnm-grunt-workaround

COPY ./files/scripts/runtime_variables_enketo_express.source.bash /etc/profile.d/runtime_variables_enketo_express.source.bash.sh
COPY ./files/enketo_express/config.json /srv/tmp/enketo_express_config.json
COPY ./files/scripts/enketo_express_copy_config.bash /etc/my_init.d/01_enketo_express_copy_config.bash
