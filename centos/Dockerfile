# FROM centos 
FROM  centos:7

# runs any  linux command 
RUN yum  install  telnet  -y  \
    yum install  unzip      -y  \
    yum  install  httpd  -y  
     
# Open containers port
EXPOSE 80      

# Copy file from host and add it to  /tmp in containe r
COPY  install.sh    get-docker.sh     /tmp

# Download from the internet add it to  /tmp
ADD    https://wordpress.org/wordpress-6.2.tar.gz       /tmp  

# Run this command when container executed, unless user  overwrite 
ENTRYPOINT  ["/usr/sbin/httpd","-D","FOREGROUND"] 