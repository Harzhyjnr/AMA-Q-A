# Use an Nginx base image to serve static files
FROM nginx:alpine

# Set working directory to /usr/share/nginx/html
WORKDIR /usr/share/nginx/html

# Remove default Nginx static files
RUN rm -rf ./*

# Copy all project files from the repository to the container
COPY . .

# Expose port 80 for web access
EXPOSE 80

# Start Nginx
CMD ["nginx", "-g", "daemon off;"]
