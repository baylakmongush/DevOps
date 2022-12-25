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
We use port 8899 in the nginx.conf file. We can change it to any port we want.

## How to run

```docker build -t demoapp:latest .```

```docker run --rm -it -p 8899:8899 -d demoapp:latest```

After that, you can access the app at http://localhost:8899

We see the following:

![](..//Images/Example.png)