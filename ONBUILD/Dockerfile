FROM almalinux:9.2
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
# This "ONBUILD" instruction runs only, when any user uses your image
ONBUILD COPY index.html /usr/share/nginx/html/index.html 
CMD [ "nginx", "-g", "daemon off;" ]