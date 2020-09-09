ARG ELK_VERSION
FROM docker.elastic.co/elasticsearch/elasticsearch:${ELK_VERSION}

ARG ELK_VERSION

ARG INSTALL_ANALYSIS_IK=false
RUN if [ $INSTALL_ANALYSIS_IK = true ]; then \
    sh -c '/bin/echo -e "y" | /usr/share/elasticsearch/bin/elasticsearch-plugin install https://github.com/medcl/elasticsearch-analysis-ik/releases/download/v${ELK_VERSION}/elasticsearch-analysis-ik-${ELK_VERSION}.zip' \ 
;fi

EXPOSE 9200 9300
