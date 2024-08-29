FROM ruby:3.2.2

WORKDIR /app

# Gemfileとbundleのインストール
COPY Gemfile /app/Gemfile
COPY Gemfile.lock /app/Gemfile.lock
RUN bundle install

# アプリケーションコードのコピー
COPY . /app

# Railsサーバーの起動
CMD ["rails", "server", "-b", "0.0.0.0"]


