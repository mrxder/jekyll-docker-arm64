  
FROM arm64v8/ruby:2.7.3-buster

MAINTAINER mrxder <matthias@keim.dev>

RUN apt-get update && \
apt-get install -y build-essential  && \
apt-get install -y zlib1g-dev && \
gem install jekyll bundler html-proofer && \
mkdir /var/jekyll


EXPOSE 4000


WORKDIR /var/jekyll