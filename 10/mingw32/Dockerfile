FROM fedora:41
RUN dnf update -y && \
  dnf install -y mingw32-gcc-c++ mingw32-SDL2 mingw32-SDL2-static ccache cmake git ninja-build dnf-plugins-core mingw32-yaml-cpp mingw32-libpng mingw32-openal-soft && \
  dnf clean all --enablerepo=\*
