FROM  robobeerun/nexus:v3.13.0-r.1
LABEL maintainer "Erwin Mueller <erwin.mueller@deventm.com>"

USER root

ADD keycloak.json ${SONATYPE_DIR}/nexus/etc/keycloak.json

USER nexus

WORKDIR ${NEXUS_DATA}

CMD ["/opt/sonatype/start-nexus-repository-manager.sh"]

ENTRYPOINT ["/docker-entrypoint.sh"]
