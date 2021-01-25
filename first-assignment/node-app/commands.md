- docker build .

- docker run -p 8000:3000 IMG_ID

- docker run --name nodeapp IMG_ID

- docker stop nodeapp

- docker run nodeapp

- docker rm nodeapp

- docker rmi IMG_ID

- docker build -t node-demo:latest .

- docker run -p 8000:3000 -d --name nodeapp --rm node-demo:latest

- docker stop nodeapp