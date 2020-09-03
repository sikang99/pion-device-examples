#
# Makefile for rtp-send
#
PROG=rtp-send

all:
	@echo "usage: make [send|play]"

send:
	./$(PROG) localhost:5000

play-gst pg:
	gst-launch-1.0 udpsrc port=5000 caps=application/x-rtp,encode-name=VP8 \
    	! rtpvp8depay ! vp8dec ! videoconvert ! autovideosink

play-vlc pv:
	vlc ./vp8.sdp
