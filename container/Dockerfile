FROM ubuntu:latest

ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update -y
RUN apt-get upgrade -y
RUN apt-get install -y  \
  build-essential \
  curl \
  gcc \
  gdb \
  git \
  nodejs \
  python3-dev  \
  python3-venv \
  unzip \
  wget  \
  vim   \
  zsh

# python
RUN python3 -m venv /opt/venv
ENV PATH="/opt/venv/bin:$PATH"
RUN pip install unicorn==2.1.0
RUN pip install gmpy2 ptrlib pwntools pycryptodome sympy

CMD ["/usr/bin/zsh"]

