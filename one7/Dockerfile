FROM ubuntu:16.04 

RUN apt-get update
RUN apt-get install -y curl wget
COPY local.sh .
RUN chmod u+x local.sh
CMD ["/bin/bash"]
