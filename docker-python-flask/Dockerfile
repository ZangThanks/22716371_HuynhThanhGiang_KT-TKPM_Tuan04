# Base image
FROM python:3.9

# Set working directory
WORKDIR /app

# Copy file requirements trước (tối ưu cache)
COPY requirements.txt .

# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy source code
COPY . .

# Expose port
EXPOSE 5000

# Run app
CMD ["python", "app.py"]