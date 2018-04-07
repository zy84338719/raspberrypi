FROM hypriot/rpi-alpine:3.5

RUN apk add --no-cache --virtual transmission-daemon

CMD /usr/bin/transmission-daemon -f

EXPOSE 9091 51413
VOLUME ["config", "downloads", "watchdir", "incomplete"]
