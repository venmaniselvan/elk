FROM docker.elastic.co/logstash/logstash:6.3.0
RUN mkdir -p /usr/share/logstash/jms/
COPY *.jar /usr/share/logstash/jms/
COPY jms.yml /usr/share/logstash/jms/
RUN bin/logstash-plugin install logstash-input-jms
RUN ls -ltra /usr/share/logstash/jms/
