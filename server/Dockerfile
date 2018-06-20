FROM getter/golang-base:v1.10.2

ENV GOPATH /opt/go/

RUN mkdir -p /opt/go/src && cd /opt/go/src && git clone https://github.com/yogetter/MonitorOpenStackVM && \
	cd MonitorOpenStackVM/server && go get && go build

ADD server /

CMD ["/server"]
