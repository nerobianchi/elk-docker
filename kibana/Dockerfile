# FROM kibana:latest

# # RUN /opt/kibana/bin/kibana plugin --install elasticsearch/graph/latest
# # RUN /opt/kibana/bin/kibana plugin --install elastic/sense


# RUN /usr/share/kibana/bin/kibana-plugin install x-pack


# RUN chown -R kibana:kibana /usr/share/kibana
# RUN chown -R kibana:kibana /usr/share/kibana/bin/kibana
# RUN chown -R kibana:kibana /opt/kibana

# COPY ./kibana.yml /usr/share/kibana/config/kibana.yml

# ENV ELASTICSEARCH_URL "http://elasticsearch:9200"

# EXPOSE 5601:5601



FROM docker.elastic.co/kibana/kibana:5.2.1
ENV ELASTICSEARCH_URL "http://elasticsearch:9200"