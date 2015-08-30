FROM maxexcloo/nginx-php:latest
MAINTAINER Sebastian Feuerstack <Sebastian@Feuerstack.org>
ENV VERSION 2.14.3
RUN mkdir -p /data/http && \
	cd /data/http && \
	wget  "http://builds.piwik.org/piwik.zip" && \	
	unzip piwik -d /tmp && \
	cp -r /tmp/piwik/* . && \
	cp  /tmp/piwik/.??* . && \
	rm -rf /tmp/piwik piwik.zip && \
	chown -R core:core .
#	rm -rf *.md .coveralls.yml ChangeLog composer.json config.sample.inc.php DCO doc examples phpunit.* README RELEASE-DATE-* setup
ADD data /data
