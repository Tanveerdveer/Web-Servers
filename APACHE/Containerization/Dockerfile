\# Use the official Ubuntu as a base image\
FROM ubuntu:20.04\
\
\# Set environment variables to non-interactive (so it doesn't ask questions during package install)\
ENV DEBIAN\_FRONTEND=noninteractive\
\
\# Update the package list and install Apache (httpd)\
RUN apt-get update && \\\
    apt-get install -y apache2 && \\\
    apt-get clean\
\
\# Expose port 80 to the outside world (HTTP port)\
EXPOSE 80\
\
\# Start Apache when the container runs\
CMD \["apache2ctl", "-D", "FOREGROUND"]
