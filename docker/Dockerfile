FROM odise/busybox-python

MAINTAINER Alex Didenko version: 0.1

COPY server.py /usr/bin/server.py

ENV NETCHECK server

CMD ["/bin/python", "/usr/bin/server.py", "8081", "0.0.0.0"]
