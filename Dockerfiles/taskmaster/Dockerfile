# Dockerfile for the 'Task' tool (taskfile.dev)

# Start from a minimal Alpine base image
FROM alpine:3.20

# Install curl so we can download the installer script
RUN apk add --no-cache curl

# Download and run the official installation script.
# This will download the correct binary for this architecture
# and place it in /usr/local/bin/, which is already in the PATH.
RUN sh -c "$(curl --location https://taskfile.dev/install.sh)" -- -d

# Optional: Verify the installation
RUN task --version