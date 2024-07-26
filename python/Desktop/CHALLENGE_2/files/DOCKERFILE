# Use a lightweight base image
FROM python:3.9-slim

# Set the working directory in the container
WORKDIR /app

# Copy the current directory content into the container at /app
COPY . /app

# Install any needed packages specified in requirements.txt
RUN pip install --no-cache-dir-r requirements.txt

# Make port 7001 available to the world outside this container
EXPOSE 7001

# Define Environment variable
ENV NAME world

# RUN app.py when the container launches
CMD ["python", "app.py"]
