# Use the latest Ubuntu image as the base image
FROM ubuntu:latest

# Set the environment variable for non-interactive installation
ENV DEBIAN_FRONTEND=noninteractive

# Update APT, upgrade installed packages, and install python3, python3-pip
RUN apt-get update && apt-get upgrade -y && \
    apt-get install -y python3 python3-pip

# Install Flask using pip3
RUN pip3 install flask

# Set the working directory in the container to /app
WORKDIR /app

# Copy the api.py file from the local machine to the Docker image at /app
COPY api.py /app

# Expose port 5252 for the Flask app
EXPOSE 5252

# Command to run the Flask app
CMD ["python3", "api.py"]
