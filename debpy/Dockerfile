FROM debian

RUN \
#Update Repository
apt update && \

#Install python3 and pip3
apt docker install python3 python3-pip -y && \

#clear cache packages
apt-get clean autoclean && \
apt-get autoremove --yes && \
rm -rf /var/lib/{apt,dpkg,cache,log}/

ENTRYPOINT /usr/bin/python3
