FROM jitsi/base-java

RUN \
	apt-dpkg-wrap apt-get update && \
	apt-dpkg-wrap apt-get install -y procps jitsi-videobridge && \
	apt-cleanup

COPY rootfs/ /

VOLUME /config

EXPOSE 10000/udp 4443
