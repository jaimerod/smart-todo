# docker/nginx/Dockerfile

FROM nginx:alpine
WORKDIR /var/www

# Initialize
RUN apk update && apk upgrade

# Install Node
RUN apk add --no-cache python3 py3-pip g++ make "nodejs>=14.17.1-r0" "npm>=7.17.0-r0"
RUN npm run dev

CMD ["nginx"]
EXPOSE 80
