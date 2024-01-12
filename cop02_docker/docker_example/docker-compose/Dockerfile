FROM ubuntu:20.04

RUN apt update
RUN apt upgrade -y

RUN yes | unminimize

# Enable ssh into the container and other basic packages
# iproute2 : Install ip command
# iputils-ping: Install ping command
# tree: displays directories and subdirectories visually
RUN apt-get install -y software-properties-common openssh-server iproute2 iputils-ping sudo curl vim less tree nano mlocate man-db manpages-posix cpio

# Enable password authentication
RUN echo 'root:secret' | chpasswd
RUN sed -i 's/PermitRootLogin prohibit-password/PermitRootLogin yes/' /etc/ssh/sshd_config
RUN sed -i 's/^#PermitRootLogin yes/PermitRootLogin yes/' /etc/ssh/sshd_config
RUN sed -i 's/^#PasswordAuthentication yes/PasswordAuthentication yes/' /etc/ssh/sshd_config
RUN sed 's@session\s*required\s*pam_loginuid.so@session optional pam_loginuid.so@g' -i /etc/pam.d/sshd
RUN mkdir /var/run/sshd
RUN service ssh force-reload
RUN service ssh restart
RUN useradd -m ctl -s /bin/bash -G sudo -p $(openssl passwd secret)

WORKDIR /home/ctl

EXPOSE 22
ENTRYPOINT ["/lib/systemd/systemd"]
CMD ["/usr/sbin/sshd", "-D"]