FROM nginx:alpine
WORKDIR /usr/share/nginx/html

# Remove default files
RUN rm -rf ./*

# Copy your React build output to nginx html folder
COPY build/ .   # make sure you've run "npm run build" first

# Optionally copy your own nginx.conf
COPY nginx.conf /etc/nginx/nginx.conf

EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
