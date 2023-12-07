FROM node:21-alpine as builder
WORKDIR /app


COPY . .
RUN npm install
RUN npm run build --prod


FROM nginx:1.23.2-alpine 
ENV NODE_ENV production


COPY --from=builder /app/dist/* /usr/share/nginx/html



EXPOSE 80