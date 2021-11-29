# Base Image Def.
FROM ubuntu:16.04

# Update the APT Repo.
RUN apt-get update 

#Install Apache Packages 
RUN apt-get install apache2 -y 

# Deploy Custom Web Page
COPY index.html /var/www/html/index.html

# Expose Port
EXPOSE 80

# Start Apache Service
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]
