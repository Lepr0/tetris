# Tetris
Tetris game built on HTML5 Canvas and Javascript. Built mostly as a learning exercise for array matrixes and how to manipulate them.
[Live app](https://tetris.leprolab.ru)

## Getting Started
Running the game is simple:
### Prebuilt Docker image
```sh
docker run -d -p 8080:80 --name tetris lepr0/tetris
```
### Nginx Docker volume mounts
```sh
git clone https://github.com/Lepr0/tetris
cd tetris
docker run --name tetris -v ./html:/usr/share/nginx/html:ro -d -p 8080:80 nginx:stable-alpine-slim
```

### Docker-compose on localhost:8080
```sh
git clone https://github.com/Lepr0/tetris
cd tetris
docker-compose up -d
```

### Standalone Local
```sh
git clone https://github.com/Lepr0/tetris
cd tetris
sudo cp html /usr/share/nginx/html
```
Once downloaded and place in a web server directory, open it in your browser

