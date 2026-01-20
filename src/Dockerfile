# Emscripten + Meson build
FROM emscripten/emsdk:3.1.57

# Disable interactive prompts
ARG DEBIAN_FRONTEND=noninteractive

# Install Meson and Ninja
RUN apt-get update \
 && apt-get install -y --no-install-recommends python3-pip ninja-build \
 && rm -rf /var/lib/apt/lists/* \
 && pip3 install --no-cache-dir meson==1.10.1
