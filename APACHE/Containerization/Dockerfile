\# Use an official Debian base image

FROM debian:latest

\# Set environment variables

ENV DEBIAN\_FRONTEND=noninteractive

\# Install Apache2

RUN apt-get update && \\

    apt-get install -y apache2 && \\

    apt-get clean && \\

    rm -rf /var/lib/apt/lists/\*

\# Copy a custom index.html to the Apache default directory (optional)

\# COPY index.html /var/www/html/

\# Expose port 80 to the outside world

EXPOSE 80

\# Start Apache2 service

CMD \["apachectl", "-D", "FOREGROUND"]

