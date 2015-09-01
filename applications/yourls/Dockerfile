FROM maxexcloo/nginx-php:latest
MAINTAINER Sebastian Feuerstack <Sebastian@Feuerstack.org>
ENV VERSION 1.7
RUN mkdir -p /data/http && \
	cd /data/http && \
	wget -O - "https://github.com/YOURLS/YOURLS/archive/1.7.tar.gz" | tar --strip-components=1 -x -z 

#ADD data /data
