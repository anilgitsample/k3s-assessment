# Use official lightweight Nginx image
FROM nginx:1.27-alpine

# Remove default Nginx web page
RUN rm -rf /usr/share/nginx/html/*

# Copy our custom Hello World page
COPY index.html /usr/share/nginx/html/index.html

# Expose HTTP port
EXPOSE 80

# Start Nginx in foreground
CMD ["nginx", "-g", "daemon off;"]
