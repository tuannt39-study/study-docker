FROM centos:8.2.2004
RUN yum update -y \
  && yum install httpd httpd-tools vim epel-release -y \
  && yum update -y \
  && yum install htop -y
EXPOSE 80
ADD . /var/www/html
ENTRYPOINT ["/usr/sbin/httpd", "-D", "FOREGROUND"]