FROM arm/prom/node-exporter:v0.16.0

ENV NODE_ID=none

USER root

COPY conf /etc/node-exporter/

COPY qemu-arm-static /usr/bin

ENTRYPOINT  [ "/etc/node-exporter/docker-entrypoint.sh" ]
CMD [ "/bin/node_exporter" ]
