#Start from ubuntu 22.04 image
FROM ubuntu:22.04

#Install curl
RUN apt-get update 
RUN apt-get -y install curl

# Copy the script.sh file from this directory
COPY script.sh .

# Add execution permissions during the build.
RUN chmod +x script.sh

# When running docker run the command will be ./script.sh
CMD ./script.sh
