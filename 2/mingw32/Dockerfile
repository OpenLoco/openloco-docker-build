FROM fedora:35
RUN dnf update -y && \
  dnf install -y mingw32-SDL2 mingw32-SDL2-static mingw32-SDL2_mixer ccache cmake git ninja-build dnf-plugins-core mingw32-yaml-cpp mingw32-libpng mingw32-openal-soft && \
  dnf clean all --enablerepo=\*
