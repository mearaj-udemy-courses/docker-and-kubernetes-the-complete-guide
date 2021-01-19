FROM node:14.15.4 as builder
WORKDIR '/app'
COPY package.json .
RUN npm install
COPY . .
RUN npm run build

FROM nginx:1.9.8
COPY --from=builder /app/build /usr/share/nginx/html