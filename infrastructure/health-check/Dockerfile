FROM node:25.7.0-slim
LABEL MAINTAINER "Madhu Akula" INFO="Kubernetes Goat"

WORKDIR /app

COPY code .

RUN apt update && apt install wget iputils-ping -y \
    && npm install

EXPOSE 80

CMD ["npm", "start"]
