# Use official Nginx image
FROM nginx:alpine

# Copy custom nginx config
COPY docker/default.conf /etc/nginx/conf.d/default.conf

# Copy website content to nginx html folder
COPY html/ /usr/share/nginx/html/

# Expose port
EXPOSE 80

# Start Nginx
CMD ["nginx", "-g", "daemon off;"]