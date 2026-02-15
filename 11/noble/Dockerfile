FROM ubuntu:24.04

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
        ninja-build \
        pkg-config \
    && update-ca-certificates \
    && rm -rf /var/lib/apt/lists/*
RUN git clone --depth=1 https://github.com/libsdl-org/SDL.git \
    && cd SDL \
    && git checkout a962f40bbba175e9716557a25d5d7965f134a3d3 \
    && mkdir build \
    && cd build \
    && cmake .. \
    && cmake --build . \
    && cmake --install .

