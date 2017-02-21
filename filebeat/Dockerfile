FROM ubuntu

RUN apt-get update && apt-get install -y curl

RUN curl -L -O https://artifacts.elastic.co/downloads/beats/filebeat/filebeat-5.2.1-amd64.deb && dpkg -i filebeat-5.2.1-amd64.deb

COPY ./config/filebeat.yml /etc/filebeat/filebeat.yml

CMD ["/usr/bin/filebeat", "-c", "/etc/filebeat/filebeat.yml -e"]
