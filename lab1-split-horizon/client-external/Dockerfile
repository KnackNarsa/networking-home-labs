#client machines

FROM ubuntu:22.04

RUN apt-get update && \
apt-get install -y dnsutils iputils-ping curl traceroute \
rm -rf /var/lib/apt/lists/*

CMD ["/bin/bash"]