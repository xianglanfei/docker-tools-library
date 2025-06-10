# Dockerfile for the 'Task' tool (taskfile.dev) - MORE ROBUST VERSION

# Start from a minimal Alpine base image
FROM alpine:3.20

# Install curl so we can download the installer script
RUN apk add --no-cache curl

# Download and run the official installation script.
# The 'sh -c' command downloads and executes the install script.
# The '-- -d -b /usr/local/bin' part is passed AS ARGUMENTS to the install script.
# -d: tells the script to just download the binary for the correct OS/architecture.
# -b /usr/local/bin: tells the script where to place the final 'task' binary.
# This location is already in the system's PATH.
RUN sh -c "$(curl --location https://taskfile.dev/install.sh)" -- -d -b /usr/local/bin

# Verify the installation was successful and the command is found
RUN task --version