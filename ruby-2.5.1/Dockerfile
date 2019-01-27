FROM ruby:2.5.1

RUN apt-get update -qq && apt-get install -y build-essential default-libmysqlclient-dev nodejs graphviz
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash - \
        && apt-get install -y nodejs
WORKDIR /var/www/html
