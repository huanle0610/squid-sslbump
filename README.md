Squid ssl-bump caching proxy
============================

A caching proxy server to selectively MITM SSL connections to cache the content. Objective is to speed up delivery rather than spy on people. 

To build: 

docker build -t jamesyale/squid-sslbump .

To run: 

docker run -d --name squid-sslbump -v /path/to/git/repo/squid-config:/etc/squid
