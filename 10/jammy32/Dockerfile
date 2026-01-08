FROM ubuntu:22.04

ENV DEBIAN_FRONTEND=noninteractive
RUN dpkg --add-architecture i386 \
    && apt-get update \
    && apt-get -y upgrade \
    && apt-get install --no-install-recommends -y \
        ca-certificates \
        ccache \
        clang \
        cmake \
        g++-multilib \
        gcc-multilib \
        git \
        libgtest-dev:i386 \
        libtbb-dev:i386 \
        libopenal-dev:i386 \
        libpng-dev:i386 \
        libsdl2-dev:i386 \
        ninja-build \
        pkg-config:i386 \
    && update-ca-certificates \
    && rm -rf /var/lib/apt/lists/*
