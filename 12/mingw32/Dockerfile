FROM fedora:43
RUN dnf update -y && \
  dnf install -y mingw32-gcc-c++ mingw32-SDL3 ccache cmake git ninja-build dnf-plugins-core mingw32-yaml-cpp mingw32-libpng mingw32-openal-soft && \
  dnf clean all --enablerepo=\*
