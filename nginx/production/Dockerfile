FROM nginx:1.13

ENV ftp_proxy http://proxy.cse.cuhk.edu.hk:8000
ENV http_proxy http://proxy.cse.cuhk.edu.hk:8000
ENV https_proxy http://proxy.cse.cuhk.edu.hk:8000

RUN mkdir -p /etc/nginx/ssl/
RUN apt-get update --fix-missing
RUN apt-get install -y openssl
RUN openssl dhparam -out /etc/nginx/ssl/dhparam.pem 2048
