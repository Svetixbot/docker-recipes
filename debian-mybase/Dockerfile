FROM debian:jessie
MAINTAINER Bruno Adelé "bruno@adele.im"

USER root
ENV DEBIAN_FRONTEND noninteractive
ENV TERM xterm-256color
ENV DISPLAY :0

# Upgrade the distribution
RUN apt-get update
RUN apt-get -yf upgrade
RUN apt-get -yf dist-upgrade

# Requirement package
RUN apt-get -y install apt-utils curl nano git

# Clean the cache and unused packages
RUN apt-get clean
RUN apt-get autoremove

CMD bash
