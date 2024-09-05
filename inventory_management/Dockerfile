# Your Solution
# Your Solution
 
# Use the official Python image as the base image
FROM python:3.9-slim
 
# Set the working directory in the container
WORKDIR /app
 
# Copy the requirements file to the container
COPY requirements.txt .
 
# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt
 
# Copy the rest of the application code to the container
COPY . .
 
# Expose the port the app runs on
EXPOSE 8001
 
# Command to run the application
CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "8001"]