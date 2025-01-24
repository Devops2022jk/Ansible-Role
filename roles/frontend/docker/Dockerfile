# Build stage
FROM node:18 AS builder
WORKDIR /app
COPY src /app
RUN npm install -g create-react-app && npm run build

# Serve stage
FROM nginx:alpine
COPY --from=builder /app/build /usr/share/nginx/html
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]

