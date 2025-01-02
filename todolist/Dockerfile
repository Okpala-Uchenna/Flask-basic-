# Use the official lightweight Python image
FROM python:3-alpine3.15

# Set the working directory inside the container
WORKDIR /app

# Copy all application files to the working directory
COPY . /app

# Install required Python packages
RUN pip install --no-cache-dir -r requirements.txt

# Expose port 3000 for the application
EXPOSE 3000

# Specify the command to run the application
CMD ["python", "./index.py"]
