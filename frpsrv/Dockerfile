# Use an official Python runtime as a parent image
FROM ubuntu:16.04

# Set the working directory to /opt
WORKDIR /opt

# Copy the current directory contents into the container at /frps
ADD opt /opt

# update system packages
RUN apt-get update

# Make port 60000-62000 available to the world outside this container
EXPOSE 60000-62000

# Define environment variable
# ENV NAME World

# Run fpcs when the container launches
CMD ["./frps", "-c", "./frps.ini"]