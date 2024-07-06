FROM node:22 as build-stage

WORKDIR /frontend-app
COPY package.json ./
RUN npm install
COPY public public
COPY src src
RUN npm run build

FROM nginx:alpine
COPY --from=build-stage /frontend-app/build /usr/share/nginx/html
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]