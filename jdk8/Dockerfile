FROM ubuntu

MAINTAINER zimmem zhuang

# download jdk manually
ADD jdk-8u60-linux-x64.tar.gz /usr/local/

WORKDIR /usr/local


RUN ln -s jdk1.8.0_60 jdk

ENV JAVA_HOME /usr/local/jdk
ENV PATH $PATH:$JAVA_HOME/bin

CMD ["java", "-version"]
