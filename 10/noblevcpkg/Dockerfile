FROM ubuntu:24.04

ENV DEBIAN_FRONTEND=noninteractive
RUN dpkg --add-architecture i386 \
    && apt-get update \
    && apt-get -y upgrade \
    && apt-get install --no-install-recommends -y \
        autoconf \
        automake \
        ca-certificates \
        ccache \
        clang \
        clang-tidy \
        cmake \
        curl \
        g++-multilib \
        gcc-multilib \
        git \
        libtool \
        make \
        ninja-build \
        zip \
        unzip \
        pkg-config:i386 \
    && update-ca-certificates \
    && rm -rf /var/lib/apt/lists/*
