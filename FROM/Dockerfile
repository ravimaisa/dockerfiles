FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
COPY index.html /usr/share/nginx/html/index.html
CMD ["nginx", "-g", "daemon off;"]
LABEL maintainer="Ravi" version="1.0" environment="production"
EXPOSE 80 443
ENV APP_ENV=production VERSION=1.0 DEBUG=false
ADD https://www.gnu.org/graphics/gnu-head-sm.jpg /usr/share/nginx/html/gnu.jpg
