FROM ubuntu:18.04

RUN dpkg --add-architecture i386 \
    && apt-get update \
    && apt-get -y upgrade \
    && apt-get install --no-install-recommends -y \
        gpg wget ca-certificates \
    && wget -O - https://apt.kitware.com/keys/kitware-archive-latest.asc | gpg --dearmor - > /usr/share/keyrings/kitware-archive-keyring.gpg \
    && echo "deb [signed-by=/usr/share/keyrings/kitware-archive-keyring.gpg] https://apt.kitware.com/ubuntu/ bionic main" > /etc/apt/sources.list.d/kitware.list \
    && apt-get update \
    && rm /usr/share/keyrings/kitware-archive-keyring.gpg \
    && apt-get install --no-install-recommends -y \
        ccache \
        clang \
        cmake \
        g++-multilib \
        gcc-multilib \
        git \
        kitware-archive-keyring \
        libgtest-dev:i386 \
        libopenal-dev:i386 \
        libpng-dev:i386 \
        libsdl2-dev:i386 \
        libyaml-cpp-dev:i386 \
        ninja-build \
        pkg-config:i386 \
    && rm -rf /var/lib/apt/lists/*
