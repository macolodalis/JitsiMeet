ARG JITSI_REPO=jitsi
FROM ${JITSI_REPO}/base-java:unstable-2024-05-25

RUN \
	apt-dpkg-wrap apt-get update && \
	apt-dpkg-wrap apt-get install -y jitsi-videobridge2 jq curl && \
	apt-cleanup

COPY rootfs/ /

VOLUME /config
