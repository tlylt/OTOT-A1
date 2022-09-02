FROM nginx

# Remove default nginx configs to avoid conflict
RUN rm /etc/nginx/nginx.conf /etc/nginx/conf.d/default.conf

# Copy nginx config
COPY nginx.conf /etc/nginx/nginx.conf

# Create /usr/app directory
WORKDIR /usr/app

# Copy source files
COPY index.html .

# Run nginx
CMD ["nginx", "-g", "daemon off;"]