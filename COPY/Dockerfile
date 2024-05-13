# base OS
FROM almalinux:8
# installing or updating the required packages
RUN yum update -y
# installing web server
RUN yum install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
# copying app code
COPY qi/ /usr/share/nginx/html
# starting the server
CMD [ "nginx", "-g", "daemon off ;" ]