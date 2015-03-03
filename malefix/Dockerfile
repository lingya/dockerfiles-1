FROM dockerfile/java:oracle-java8
MAINTAINER Martin Coxall "martin.coxall@schneiderinvestmentassociates.com"
ADD https://raw.githubusercontent.com/technomancy/leiningen/stable/bin/lein /usr/bin/
ADD profiles.clj ~/.lein/
RUN chmod a+x /usr/bin/lein
ENV LEIN_ROOT=true
WORKDIR /data
RUN git clone https://github.com/sra-london/malefix
WORKDIR /data/malefix
RUN lein compile
