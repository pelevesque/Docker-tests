FROM ubuntu:bionic

RUN apt-get update && apt-get install -y firefox

RUN adduser --disabled-password --gecos "" --shell /bin/bash someuser
RUN usermod -g sudo someuser
RUN passwd -d someuser

USER someuser
CMD /usr/bin/firefox
