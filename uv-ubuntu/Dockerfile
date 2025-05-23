FROM ubuntu:24.04

# Set working directory
WORKDIR /workspace

# Update package lists and upgrade installed packages
RUN apt-get update && apt-get upgrade -y

# Install prerequisites for uv
RUN apt-get install -y curl ca-certificates

# Copy the latest uv binary from the official uv image
COPY --from=ghcr.io/astral-sh/uv:latest /uv /usr/local/bin/uv

# Verify uv installation
RUN uv --version

# Optional: Clean up to reduce image size
RUN apt-get clean && rm -rf /var/lib/apt/lists/*
