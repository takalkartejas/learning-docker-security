FROM ubuntu:18.04

LABEL maintainer="Tejas"

#Add a user

#tejas has sudo access
RUN groupadd -r tejas && useradd -r -g sudo tejas 
#We add alex to his own group which means he should not have any access
#If we write a random group name except alex, it will give error that group does not exist
RUN groupadd -r alex && useradd -r -g alex alex 

WORKDIR /app
ADD . .
# ENV HOME /root
# ENV DEBIAN_FRONTEND=noninteractive

RUN apt update
RUN apt install nano && apt-get -y install sudo