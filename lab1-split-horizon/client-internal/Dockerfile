#dns-client machine

FROM ubuntu:22.04

RUN apt-get update && \
apt-get install -y dnsutils iputils-ping curl traceroute && \
rm -rf /var/lib/apt/lists/*

CMD ["tail", "-f", "/dev/null"]