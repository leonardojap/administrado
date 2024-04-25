# Etapa de construcción
FROM node:20-alpine AS build
RUN npm install -g npm@10.5.0
WORKDIR /app
COPY package.json package-lock.json ./
RUN npm install
COPY . .
RUN npm run build:prod --ignore-errors

# Etapa de producción
FROM nginx:alpine AS prod
COPY --from=build /app/dist/courses/browser /usr/share/nginx/html
COPY nginx.conf /etc/nginx/conf.d/default.conf
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
