# Use the latest version of Ubuntu as a parent image
FROM ubuntu:latest

# Update the package lists and upgrade all the installed packages
RUN apt-get update && apt-get upgrade -y && rm -rf /var/lib/apt/lists/*

# When the Docker container is run, echo "Hello, World!"
CMD ["echo", "Hello, World!"]
