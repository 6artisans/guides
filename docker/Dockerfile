FROM ruby:2.2.3

ENV APP_HOME /app
RUN mkdir $APP_HOME
WORKDIR $APP_HOME

ADD avvoka_app/Gemfile* $APP_HOME/
RUN bundle install
