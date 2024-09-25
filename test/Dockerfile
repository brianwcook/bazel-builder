FROM quay.io/bcook/bazel:ubi8-bazel-5
RUN dnf -y install gcc-c++ git
COPY source source
RUN pwd && cd /source/test/source && ls && bazel build //main:hello-world
