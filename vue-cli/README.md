# Docker image inglebard/vue-cli
Vue Cli
[Github](https://github.com/Inglebard/dockerfiles/tree/master/vue-cli)
[Dockerhub](https://hub.docker.com/r/inglebard/vue-cli)

## Why use this image :

This image was created to develop vue app.

## Technical information :

### Softwares :
* node
* npm
* vue-cli

### Ports :
* 8080

### Volumes :
You may need to mount app folder to /var/www/html.

## How to use this image :

You can create a project :
```
docker run -it -v vue_app:/var/www/html inglebard/vue-cli:latest vue init webpack-simple .
```

You can serve the project like this:
```
docker run -it -v vue_app:/var/www/html -p 4200:4200 inglebard/vue-cli:latest

```

## Note :

The default command is `npm run dev`.