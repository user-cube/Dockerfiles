# Deployment of NestJS Containers

This folder contains Dockerfile information to build NestJS apps.

## Bcrypt

If you're using `bcrypt` library you may face some troubles because of node-alpine. Add the following lines to builder:

```Dockerfile
RUN apk --no-cache add --virtual builds-deps build-base python
RUN npm config set python /usr/bin/python
```
