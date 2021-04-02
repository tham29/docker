ARG ELK_VERSION

# https://github.com/elastic/logstash-docker
FROM elastic/filebeat:7.12.0
COPY config/filebeat.yml /usr/share/filebeat/filebeat.yml
USER root
RUN mkdir /usr/share/filebeat/dockerlogs
RUN chown  root /usr/share/filebeat/filebeat.yml
RUN chmod  go-w /usr/share/filebeat/filebeat.yml
