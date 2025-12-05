FROM docker.elastic.co/elasticsearch/elasticsearch:8.6.2

COPY jaso-analyzer-plugin-8.6.2-plugin.zip /tmp/jaso-analyzer-plugin-8.6.2-plugin.zip
RUN bin/elasticsearch-plugin install --batch analysis-nori
RUN bin/elasticsearch-plugin install --batch file:///tmp/jaso-analyzer-plugin-8.6.2-plugin.zip
