FROM verdaccio/verdaccio:4

USER root

ENV NODE_ENV=production

RUN npm i

RUN npm install @verdaccio/local-storage

# COPY config.yaml /verdaccio/conf/config.yaml

# RUN /bin/chown -R 10001:65533 /verdaccio

RUN ls -l /verdaccio/conf

# COPY config.yaml /verdaccio/conf/config.yaml 

# RUN ls -l /verdaccio/conf

# RUN /opt/verdaccio -c /verdaccio/conf/config.yaml

# CMD ["verdaccio", "-c", "/verdaccio/conf/config.yaml"]

USER verdaccio