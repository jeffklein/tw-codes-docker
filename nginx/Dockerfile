FROM nginx:1.9.0

RUN  mkdir /etc/nginx/ssl
COPY ./invitecodes.net.pem /etc/nginx/ssl/invitecodes.net.pem
COPY ./invitecodes.net.key /etc/nginx/ssl/invitecodes.net.key
RUN  chmod -R 600 /etc/nginx/ssl
RUN  rm -f /etc/nginx/conf.d/default.conf
#RUN  rm -f /etc/nginx/conf.d/example_ssl.conf
COPY ./nginx.conf /etc/nginx/conf.d/nginx-ssl.conf
