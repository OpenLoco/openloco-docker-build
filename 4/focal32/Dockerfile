FROM ubuntu:20.04

ENV DEBIAN_FRONTEND=noninteractive
RUN dpkg --add-architecture i386 \
    && apt-get update \
    && apt-get -y upgrade \
    && apt-get install --no-install-recommends -y \
        gpg wget ca-certificates \
    && wget -O - https://apt.kitware.com/keys/kitware-archive-latest.asc | gpg --dearmor - > /usr/share/keyrings/kitware-archive-keyring.gpg \
    && echo "deb [signed-by=/usr/share/keyrings/kitware-archive-keyring.gpg] https://apt.kitware.com/ubuntu/ focal main" > /etc/apt/sources.list.d/kitware.list \
    && apt-get update \
    && rm /usr/share/keyrings/kitware-archive-keyring.gpg \
    && apt-get install --no-install-recommends -y \
        ca-certificates \
        ccache \
        clang \
        cmake \
        g++-multilib \
        gcc-multilib \
        git \
        kitware-archive-keyring \
        libgtest-dev \
        libopenal-dev:i386 \
        libpng-dev:i386 \
        libsdl2-dev:i386 \
        ninja-build \
        pkg-config:i386 \
    && update-ca-certificates \
    && rm -rf /var/lib/apt/lists/*
