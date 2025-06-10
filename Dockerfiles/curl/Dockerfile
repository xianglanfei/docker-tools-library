# Dockerfile for the 'curl' tool

# Start from the latest stable version of Alpine Linux.
FROM alpine:3.20

# Use the Alpine package manager to install the 'curl' package.
# We also install 'ca-certificates' which are required for 'curl'
# to make secure HTTPS requests.
RUN apk add --no-cache curl ca-certificates