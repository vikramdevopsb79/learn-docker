# Use an official RHEL 9 UBI as a parent image
FROM registry.access.redhat.com/ubi9/ubi:latest

# Install debugging tools
RUN dnf update -y && \
    dnf install -y curl wget vim nano net-tools iputils bind-utils strace lsof && \
    dnf clean all
