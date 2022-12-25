FROM node:16-alpine as builder

WORKDIR /builddir
COPY package*.json ./

RUN npm install

COPY . ./

RUN npm run build

FROM nginx:1.15

COPY --from=builder /builddir/build /usr/share/nginx/html

COPY nginx.conf /etc/nginx/conf.d/default.conf