# Use the latest Ubuntu image as the base image
FROM ubuntu:latest

# Set the environment variable for non-interactive installation
ENV DEBIAN_FRONTEND=noninteractive

# Update APT and upgrade installed packages
RUN apt-get update && apt-get upgrade -y

# Command to run when the container starts
CMD echo "Hello, World!"
