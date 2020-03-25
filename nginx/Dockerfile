FROM nginx
COPY cert/yinsheng.studio/3655740_yinsheng.studio.key /etc/nginx/cert/
COPY cert/yinsheng.studio/3655740_yinsheng.studio.pem /etc/nginx/cert/
COPY cert/yinshengphy.cn/3525679_yinshengphy.cn.key /etc/nginx/cert/
COPY cert/yinshengphy.cn/3525679_yinshengphy.cn.pem /etc/nginx/cert/
COPY conf.nginx /etc/nginx/nginx.conf
COPY favicon.ico /usr/share/nginx/html/
RUN echo "<h1>Welcome To Yinsheng' Docker</h1>" > /usr/share/nginx/html/index.html
VOLUME /usr/share/nginx/html