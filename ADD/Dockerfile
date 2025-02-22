FROM almalinux:9.2
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
ADD https://raw.githubusercontent.com/Prasadraju99/terraform-aws-ec2/refs/heads/main/ec2.tf /usr/share/nginx/html/index.html
RUN chmod 775  /usr/share/nginx/html/index.html
CMD [ "nginx", "-g", "daemon off;" ]