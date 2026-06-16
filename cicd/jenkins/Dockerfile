FROM jenkins/jenkins:lts-jdk21
ENV JAVA_OPTS="-Djenkins.install.runSetupWizard=false"
RUN jenkins-plugin-cli --plugins "workflow-aggregator git docker-workflow"
COPY security.groovy /usr/share/jenkins/ref/init.groovy.d/security.groovy
