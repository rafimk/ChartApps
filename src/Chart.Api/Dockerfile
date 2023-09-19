FROM python:3.9-slim-buster

# Set the working directory to /app
WORKDIR /app

# Copy the current directory contents into the container at /app
COPY . /app

# Install any needed packages specified in requirements.txt
RUN pip install --trusted-host pypi.python.org -r requirements.txt

# Make port 80 available to the world outside this container

# Define environment variable
ENV NAME World
ENV URL_PREFIX = "http://localhost"

ENV API_PORT=5001

# Expose the API port
EXPOSE $API_PORT

# Run app.py when the container launches
CMD ["python", "app.py"]