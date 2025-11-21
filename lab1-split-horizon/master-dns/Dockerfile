# master-dns/Dockerfile

FROM debian:stable-slim

RUN apt-get update && \
apt-get install -y bind9 bind9utils dnsutils sudo vim \ 
rm -rf /var/lib/apt/lists/*

RUN useradd -m -s /bin/bash dnsadmin && \
echo "dnsadmin ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/dnsadmin

RUN mkdir -p /lab-templates /etc/bind/zones

COPY templates/ /lab-templates/

EXPOSE 53/udp 53/tcp

CMD ["/usr/sbin/named, "-f", "-u", "bind", "-c" "/etc/bind/named.conf"]

