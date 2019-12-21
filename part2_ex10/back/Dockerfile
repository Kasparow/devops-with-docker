FROM ubuntu:16.04 

RUN apt-get update
RUN apt-get install -y curl wget
RUN apt-get install -y git
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN git clone https://github.com/docker-hy/backend-example-docker.git
WORKDIR /backend-example-docker
RUN apt install -y nodejs
RUN npm install

CMD ["/bin/bash"]
# ENV FRONT_URL=http://localhost:5000
ENTRYPOINT npm start
