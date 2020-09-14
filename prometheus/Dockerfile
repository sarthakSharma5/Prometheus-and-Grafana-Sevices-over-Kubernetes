FROM centos
RUN yum install wget -y
RUN wget https://github.com/prometheus/prometheus/releases/download/v2.21.0/prometheus-2.21.0.linux-amd64.tar.gz
RUN tar -xzf prometheus-2.21.0.linux-amd64.tar.gz
RUN mkdir /etc/prometheus
RUN cp -rf prometheus-2.21.0.linux-amd64/* /etc/prometheus
RUN cp /etc/prometheus/prometheus /usr/bin
CMD prometheus --config.file=/etc/prometheus/prometheus.yml

