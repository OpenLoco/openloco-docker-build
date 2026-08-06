FROM ubuntu:26.04

ENV DEBIAN_FRONTEND=noninteractive
RUN dpkg --add-architecture i386 \
    && apt-get update \
    && apt-get -y upgrade \
    && apt-get install --no-install-recommends -y \
        autoconf \
        autoconf-archive \
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
        libltdl-dev \
        make \
        ninja-build \
        python3-venv \
        zip \
        unzip \
        pkg-config:i386 \
        libx11-dev \
        libxcursor-dev \
        libxi-dev \
        libxrandr-dev \
        libxtst-dev \
        libxft-dev \
        libxext-dev \
        libwayland-dev \
        libxkbcommon-dev \
        libegl1-mesa-dev \
    && update-ca-certificates \
    && rm -rf /var/lib/apt/lists/*
