# Use an official Nginx image with OpenSSL installed
FROM nginx:alpine

# Copy your certificates to the container
COPY certs/cert.pem /etc/ssl/certs/
COPY certs/key.pem /etc/ssl/private/

# Copy your web app files into the container
COPY app/ /usr/share/nginx/html

# Copy the custom Nginx configuration
COPY nginx.conf /etc/nginx/nginx.conf

# Expose port 443 for HTTPS
EXPOSE 443

# Start Nginx
CMD ["nginx", "-g", "daemon off;"]
