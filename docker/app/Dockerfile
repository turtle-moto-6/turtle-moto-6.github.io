FROM debian:13
RUN apt-get update && \
    apt-get install ruby-full build-essential zlib1g-dev -y

RUN echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc && \
    echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc && \
    echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc

RUN gem install jekyll bundler

WORKDIR /app

CMD bundle install && bundle exec jekyll serve --host 0.0.0.0
