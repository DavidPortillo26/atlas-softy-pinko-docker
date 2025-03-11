# Use the latest version of Ubuntu as a parent image
FROM ubuntu:latest

# Update the package lists, upgrade all installed packages, install Python3, pip3, Flask, and Flask-Cors
RUN apt-get update && \
    apt-get upgrade -y && \
    apt-get install -y python3 python3-pip && \
    pip3 install flask flask-cors && \
    rm -rf /var/lib/apt/lists/*

# Set the working directory to /app
WORKDIR /app

# Copy the current directory contents into the container at /app
COPY . /app

# Make port 5252 available to the world outside this container
EXPOSE 5252

# Run api.py when the container launches
CMD ["python3", "api.py"]
