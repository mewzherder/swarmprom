FROM prom/alertmanager:v0.8.0

ENV SLACK_URL=none \
    SLACK_CHANNEL=general \
    SLACK_USER=alertmanager

COPY conf /etc/alertmanager/

ENTRYPOINT  [ "/etc/alertmanager/docker-entrypoint.sh" ]
CMD        [ "-config.file=/etc/alertmanager/alertmanager.yml", \
             "-storage.path=/alertmanager" ]
