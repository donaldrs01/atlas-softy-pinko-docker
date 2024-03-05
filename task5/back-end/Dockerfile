# Specify to use the latest Ubuntu
FROM ubuntu:latest

# APT (Advanced Package Tool) update
RUN apt-get update

# Upgrade packages currently installed
RUN apt-get upgrade -y

# Install Python3 and pip3
RUN apt-get install -y python3 python3-pip

# Install Flask with pip3
RUN pip3 install Flask

# Install CORS plugin for Flask
RUN pip3 install flask-CORS

# Change the working directory
WORKDIR /app

# Copy api.py from local machine to Docker image
COPY ./api.py /app/api.py

# Run python script on startup
CMD ["python3", "/app/api.py"]