FROM ruby:2.7.3

ENV BUNDLER_VERSION=2.2.20
RUN curl -sL https://deb.nodesource.com/setup_14.x | bash -
RUN curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | apt-key add -
RUN echo "deb https://dl.yarnpkg.com/debian/ stable main" | tee /etc/apt/sources.list.d/yarn.list
RUN apt-get update -y && apt-get install -y \
  nodejs \
  yarn \
  git-core \
  vim \
  zlib1g-dev \
  build-essential \
  libssl-dev \
  default-mysql-client \
  cmake \
  libmariadb-dev

RUN gem install bundler -v $BUNDLER_VERSION

WORKDIR /rails-app
