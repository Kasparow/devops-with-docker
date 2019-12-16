FROM ruby:2.6.0

RUN apt-get update
RUN apt-get install -y curl wget
RUN apt-get install -y git
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash

COPY ./rails-example-project /ruby-example-docker
WORKDIR /ruby-example-docker

RUN apt install -y nodejs
RUN npm install
RUN gem install bundler
RUN bundle install
RUN rails db:migrate

CMD ["/bin/bash"]
ENTRYPOINT rails s
