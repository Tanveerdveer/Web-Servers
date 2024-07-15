\# Use the official Ubuntu base image

FROM ubuntu:latest

\# Set environment variables to non-interactive mode for apt-get

ENV DEBIAN\_FRONTEND=noninteractive

\# Update the package list and install necessary packages

RUN apt-get update && \\

    apt-get install -y nginx && \\

    apt-get clean

\# Copy a simple Nginx configuration file (optional)

\# ADD nginx.conf /etc/nginx/nginx.conf

\# Expose port 80 to the outside world

EXPOSE 80

\# Start Nginx in the foreground

CMD \["nginx", "-g", "daemon off;"]

