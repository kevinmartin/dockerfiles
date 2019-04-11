FROM	alpine:3.7
EXPOSE	554 8090

RUN	apk add --no-cache ffmpeg && \
	rm /usr/bin/ffprobe /usr/bin/ffmpeg /usr/bin/ffplay /usr/bin/qt-faststart && \
	rm -rf /usr/share/man/*

COPY	ffserver.conf /etc/

ENTRYPOINT	["ffserver"]
