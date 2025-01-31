FROM jamesmith0817/debian-rootfs-xfce
RUN apt update && \
    apt install supervisor* libturbojpeg* ffmpeg -y 

RUN apt install dumb-init systemd firefox* -y
RUN sudo adduser cloudreve --quiet --disabled-login --disabled-password --home /home/cloudreve --gecos ""
RUN sudo adduser alist --quiet --disabled-login --disabled-password --home /home/alist  --gecos ""
RUN sudo adduser homeassistant --quiet --disabled-login --disabled-password --home /home/homeassistant --gecos ""
RUN wget "https://github.com/cloudreve/Cloudreve/releases/download/3.8.3/cloudreve_3.8.3_linux_amd64.tar.gz" -O cloudreve.tar.gz
RUN tar -zxvf cloudreve.tar.gz -C /home/cloudreve/ && rm -rf cloudreve.tar.gz
RUN tree /home/cloudreve/
RUN chmod +x /home/cloudreve/cloudreve
RUN wget "https://github.com/AlistGo/alist/releases/download/v3.41.0/alist-linux-amd64.tar.gz" -O alist-linux-amd64.tar.gz
RUN tar -zxvf alist-linux-amd64.tar.gz -C /home/alist/ && rm -rf alist-linux-amd64.tar.gz && ln -s /home/alist/alist  /usr/bin/alist
RUN tree /home/alist/
RUN chmod +x /home/alist/alist
RUN mkdir -vp /etc/supervisor/conf.d/
COPY supervisord.conf /etc/supervisor/
COPY cloudreve.conf /etc/supervisor/conf.d/
COPY homeassistant.conf /etc/supervisor/conf.d/
COPY alist.conf /etc/supervisor/conf.d/
COPY supervisord /etc/init.d/
RUN chmod +x /etc/init.d/supervisor
RUN mkdir -p /run/systemd 
STOPSIGNAL SIGRTMIN+3
EXPOSE 8123
EXPOSE 3389
EXPOSE 5244
EXPOSE 5212
# ENTRYPOINT [ "/bin/bash" ]
CMD [ "/bin/bash" ]