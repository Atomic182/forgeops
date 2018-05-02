FROM alpine:3.5

RUN apk add --no-cache curl
RUN apk add --no-cache bash

COPY testcases /tmp
COPY forgeops-smoke-test.sh /tmp

RUN chmod +x /tmp/forgeops-smoke-test.sh

ENTRYPOINT ["/bin/bash"]
