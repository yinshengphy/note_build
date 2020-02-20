FROM jenkins/jenkins

MAINTAINER yinshengphy@gmail.com
USER root
#调整时区
RUN ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime
RUN echo  'Asia/Shanghai' > /etc/timezone
RUN mkdir -p /var/approot
RUN chown -R jenkins:jenkins /var/approot
RUN chown -R jenkins:jenkins /var/backups
USER jenkins
ADD ./backup /var/backups

#note构建结果共享
VOLUME /var/approot

#更换镜像为清华镜像
#RUN  sed -i 's/http:\/\/updates.jenkins-ci.org\/download/https:\/\/mirrors.tuna.tsinghua.edu.cn\/jenkins/g' /var/jenkins_home/updates/default.json && \
#sed -i 's/http:\/\/www.google.com/https:\/\/www.baidu.com/g' /var/jenkins_home/updates/default.json
EXPOSE 8080