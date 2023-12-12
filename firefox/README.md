docker build -t firefox . # Build constainer
docker run -ti --rm -e DISPLAY -v /tmp/.X11-unix:/tmp/.X11-unix firefox # Run container

# Note: The last command needs a proper setup for X11Forwarding.
