# This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

We use nginx to serve the static files. The nginx configuration is in the Dockerfile.

```dockerfile
FROM node:16-alpine as builder

WORKDIR /builddir
COPY package*.json ./

RUN npm install

COPY . ./

RUN npm run build

FROM nginx:1.15

COPY --from=builder /builddir/build /usr/share/nginx/html

COPY nginx.conf /etc/nginx/conf.d/default.conf
```

The nginx.conf file is as follows:

```nginx
server {
  listen 8899;

  location / {
    root /usr/share/nginx/html;
    try_files $uri /index.html;
  }
}
```
We use port 8899 in the nginx.conf file. You can change it to any port you want.

## How to build the image 

```docker build -t demoapp:latest .```

## How to push to Docker Hub

```docker login```

```docker tag demoapp:latest <logindockerhub>/demoapp:latest```

```docker push <logindockerhub>/demoapp:latest```

## How to run local image

```docker run --rm -it -p 8899:8899 -d demoapp:latest```

## How to run image from Docker Hub

```docker run --rm -it -p 8899:8899 -d <logindockerhub>/demoapp:latest```

After that, you can access the app at http://localhost:8899

We see the following:

<img width="770" alt="React-screenshot" src="https://user-images.githubusercontent.com/56039676/209478735-fc73dc49-e094-4dd4-b163-0080fb946e6e.png">
