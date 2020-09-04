#
# Makefile for simple
#
PROG=simple-new
usage: 
	@echo "usage: make [build|run] for $(PROG)"

edit e:
	vi main.go

build b:
	go build -o $(PROG)

# export SDP=<base64 of browser>
run r:
	echo $(SDP) | ./$(PROG)

clean:
	rm -f $(PROG)

open o:
	open https://jsfiddle.net/gh/get/library/pure/pion/mediadevices/tree/master/examples/internal/jsfiddle/audio-and-video
	#open http://localhost:8080/

