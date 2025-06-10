# Dockerfile for the 'jq' tool

# Start from the latest stable version of Alpine Linux, which is very small.
FROM alpine:3.20

# Use the Alpine package manager (apk) to install the 'jq' package.
# --no-cache: This is a standard optimization. It tells apk not to store the
# package index locally after the installation, keeping the final image smaller.
RUN apk add --no-cache jq