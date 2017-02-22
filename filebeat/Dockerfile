FROM ubuntu

RUN apt-get update && apt-get install -y curl
RUN apt-get install -y vim

RUN curl -L -O https://artifacts.elastic.co/downloads/beats/filebeat/filebeat-5.2.1-amd64.deb && dpkg -i filebeat-5.2.1-amd64.deb

COPY ./config/filebeat.yml /etc/filebeat/filebeat.yml

ENV PATH "$PATH:/usr/bin/"
# ENV PATH "$PATH:usr/share/filebeat/bin/"

CMD ["filebeat.sh", "-e -c", "/etc/filebeat/filebeat.yml"]
