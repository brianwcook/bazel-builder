FROM quay.io/bcook/bazel:ubi8-bazel-5
RUN dnf -y install gcc-c++ git
COPY source source
RUN cat /proc/net/dev && \
    cd source && \
    bazel build //main:hello-world
