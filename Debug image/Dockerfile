# Use an official RHEL 9 UBI as a parent image
FROM registry.access.redhat.com/ubi9/ubi:latest

# Remove conflicting packages and install debugging tools
RUN dnf update -y && \
    dnf remove -y curl-minimal && \
    dnf install -y curl wget vim nano net-tools iputils bind-utils tcpdump strace lsof && \
    dnf clean all

# Set the default command to start a shell
CMD ["/bin/bash"]
