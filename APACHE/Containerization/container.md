1.To build and run the container:

**docker build -t apache-image .
**
2.Run the container:

**docker run -d -p 8080:80 apache-image
**
Now, you should be able to visit **`http://localhost:8080`** in your browser and see the Apache server running.
