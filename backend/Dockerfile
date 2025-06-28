# --- Stage 1: build dependencies ---
FROM node:20-alpine AS deps
WORKDIR /app
COPY package*.json .
RUN npm ci --audit=false --fund=false

# --- Stage 2: build source ---
FROM node:20-alpine AS build
WORKDIR /app
COPY --from=deps /app/node_modules ./node_modules
COPY . .
RUN npm run build

# --- Stage 3: production runtime ---
FROM node:20-alpine AS prod
WORKDIR /app
ENV NODE_ENV=production
COPY --from=build /app .
EXPOSE 8080
CMD ["node", "server.js"]
