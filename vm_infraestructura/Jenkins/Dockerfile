# Usar la imagen de Jenkins con Java 17 como base
FROM jenkins/jenkins:lts-jdk17

# Cambiar a root para instalar Maven
USER root

# Instalar Maven en CentOS
RUN apt-get update && apt-get install -y maven && apt-get clean

# Cambiar el usuario de vuelta a jenkins
USER jenkins
