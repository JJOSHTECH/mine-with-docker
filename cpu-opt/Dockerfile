FROM ubuntu:22.04

WORKDIR /root/

RUN apt-get update && apt-get -qy install \
    automake \
    build-essential \
    libcurl4-openssl-dev \
    libssl-dev \
    git \
    ca-certificates \
    libjansson-dev \
    libgmp-dev \
    zlib1g-dev --no-install-recommends

RUN git clone --depth 1 https://github.com/JayDDee/cpuminer-opt.git cpuminer-multi
WORKDIR /root/cpuminer-multi

RUN ./build.sh
