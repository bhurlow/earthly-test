VERSION 0.8
FROM debian:bookworm-slim
WORKDIR /app

init:
  RUN apt-get update
  RUN apt-get install -y curl dnsutils host gnupg python3 ca-certificates make g++ git
  RUN curl -sLO https://raw.githubusercontent.com/babashka/babashka/master/install && chmod +x install && ./install
  RUN sleep 5000
  RUN bb --version