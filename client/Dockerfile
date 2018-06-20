FROM getter/golang-base:v1.10.2

ENV GOPATH /opt/go/


RUN apt-get update && apt-get install -y libvirt-dev && \
 	mkdir -p /opt/go/src && cd /opt/go/src && git clone https://github.com/yogetter/MonitorOpenStackVM && \
	cd MonitorOpenStackVM/client && go get && go build


ADD client /

CMD ["/client"]

