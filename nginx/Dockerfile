FROM nginx
COPY 3151340_yinsheng.studio.key /etc/nginx/cert/
COPY 3151340_yinsheng.studio.pem /etc/nginx/cert/
COPY conf.nginx /etc/nginx/nginx.conf
COPY favicon.ico /usr/share/nginx/html/
RUN echo "<h1>Welcome To Yinsheng' Docker</h1>" > /usr/share/nginx/html/index.html
VOLUME /usr/share/nginx/html