
## Dockerizing MongoDB

docker run --name mongodb -v data:/data/db --rm -d --network goals-net mongo

## Dockerizing Node.js Backend

- Run this code in the backend folder.
- This is for Windows only. The path shortcut for bind mount will be different for OS & Linux.

docker run --name goals-backend -v logs:/app/logs -v "$(pwd):/app" -v /app/node_modules --rm -d --network goals-net goals-node

## Dockerizing React Frontend

- Run this code in src folder.
- This is for Windows only. The path shortcut for bind mount will be different for OS & Linux.

docker run -v "$(pwd):/app/src" --name goals-frontend --rm -p 3000:3000 -it --network goals-net goals-react