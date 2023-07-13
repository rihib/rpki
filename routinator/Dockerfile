FROM nlnetlabs/routinator:latest

USER root

RUN mkdir -p /root/.rpki-cache

VOLUME [ "/root/.rpki-cache" ]

EXPOSE 3323 8323

ENTRYPOINT [ "routinator", "server", "--rtr", "0.0.0.0:3323", "--http", "0.0.0.0:8323" ]
