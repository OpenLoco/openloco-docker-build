FROM ubuntu:26.04

ENV DEBIAN_FRONTEND=noninteractive
RUN apt-get update \
    && apt-get -y upgrade \
    && apt-get install --no-install-recommends -y \
        ca-certificates \
        ccache \
        clang \
        clang-tidy \
        cmake \
        g++-multilib \
        gcc-multilib \
        git \
        libgtest-dev \
        libtbb-dev \
        libopenal-dev \
        libpng-dev \
        libsdl3-dev \
        ninja-build \
        pkg-config \
    && update-ca-certificates \
    && rm -rf /var/lib/apt/lists/*

