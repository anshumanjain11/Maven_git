FROM dockerfile/java:oracle-java8

ADD Mavengitdemo.jar /opt/Mavengitdemo/
EXPOSE 8080
WORKDIR /opt/Mavengitdemo/
CMD ["java", "-Xms512m", "-Xmx1g", "-jar", "Mavengitdemo.jar"]