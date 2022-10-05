FROM node:18-alpine
ARG PORT=3333
WORKDIR /app
COPY package*.json ./
RUN npm ci
COPY . .
EXPOSE ${PORT}
ENV PORT ${PORT}
CMD node server.js
