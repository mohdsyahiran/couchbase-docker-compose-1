FROM couchbase/server:latest AS stage_base
# FROM couchbase:latest AS stage_base 
COPY init-cbserver.sh /opt/couchbase/init/
COPY sample-data.json /opt/couchbase/init/
RUN sed -i -e 's/\r$//' /opt/couchbase/init/init-cbserver.sh
