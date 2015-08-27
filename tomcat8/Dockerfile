FROM zimmem/jdk


ENV CATALINA_HOME /usr/local/tomcat
ENV PATH $CATALINA_HOME/bin:$PATH
RUN mkdir -p "$CATALINA_HOME"
WORKDIR $CATALINA_HOME


RUN apt-get install -y curl \
    && curl http://mirrors.hust.edu.cn/apache/tomcat/tomcat-8/v8.0.26/bin/apache-tomcat-8.0.26.tar.gz  -o tomcat.tar.gz \
    && tar -xvf tomcat.tar.gz --strip-components=1 \
    && rm bin/*.bat \
    && rm tomcat.tar.gz


    
EXPOSE 8080
CMD ["catalina.sh", "run"]
