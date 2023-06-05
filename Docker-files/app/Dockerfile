FROM maven:3.8.6-openjdk-11 as ARTIFACT
RUN git clone https://github.com/rahulsoniiii/vproContainerization.git
RUN cd vproContainerization && git pull origin main
RUN cd vproContainerization && mvn install

FROM tomcat:9-jre11
LABEL Author="Rahul Soni"
RUN rm -rf /usr/local/tomcat/webapps/* 
COPY  --from=ARTIFACT vproContainerization/target/*.war /usr/local/tomcat/webapps/ROOT.war
EXPOSE 8080
CMD [ "catalina.sh", "run" ]