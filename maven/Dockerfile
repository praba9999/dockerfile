FROM komljen/jdk-oracle
MAINTAINER Alen Komljen <alen.komljen@live.com>

RUN \
  apt-get update && \
  apt-get -y install \
          maven && \
  rm -rf /var/lib/apt/lists/*
CMD mvn clean verify sonar:sonar \
     -Dsonar.projectKey=test-project \
     -Dsonar.host.url=http://localhost:9000 \
     -Dsonar.login=sqp_588d163792236937a58acf6118cc01ab8b62fc19
