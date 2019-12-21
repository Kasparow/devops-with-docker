FROM ubuntu:16.04 

RUN apt-get update
RUN apt-get install -y curl wget
RUN apt-get install -y git
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN git clone https://github.com/docker-hy/frontend-example-docker.git
WORKDIR /frontend-example-docker
RUN apt install -y nodejs
RUN npm install

CMD ["/bin/bash"]
# ENV API_URL=http://localhost:8000
ENTRYPOINT npm start
