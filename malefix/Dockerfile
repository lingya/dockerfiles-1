FROM dockerfile/java:oracle-java8
MAINTAINER Martin Coxall "martin.coxall@schneiderinvestmentassociates.com"
ADD http://path.to/release.jar /opt/malefix/release.jar
ONBUILD ADD . /opt/malefix
EXPOSE <port for zookeeper>
ENTRYPOINT ["/usr/bin/java"]
CMD ["-jar" "/opt/malefix/release.jar"]
