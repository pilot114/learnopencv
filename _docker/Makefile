help:
	@echo " run"

build:
	@docker build . -t opencv_unit

run:
	@docker run --device=/dev/video0:/dev/video0 -v /tmp/.X11-unix:/tmp/.X11-unix -e DISPLAY=$DISPLAY -p 5000:5000 -p 8888:8888 -it opencv_unit /bin/bash
