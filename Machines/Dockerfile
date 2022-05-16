FROM softwareag/webmethods-microservicesruntime:10.11.0.0
MAINTAINER SoftwareAG

USER root

COPY ${PACKAGE} /opt/softwareag/IntegrationServer/packages/${PACKAGE}

COPY config /opt/softwareag/IntegrationServer/config
COPY Listeners/listeners.cnf /opt/softwareag/IntegrationServer/packages/WmRoot/config
<<<<<<< HEAD
=======
COPY acls/*.cnf /opt/softwareag/IntegrationServer/config/
>>>>>>> 63467daa2497c95e756e598a8cc02dafddc3a860

RUN chown 1724:1724 -R /opt/softwareag/IntegrationServer/packages/*

USER 1724
