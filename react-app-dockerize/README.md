# NOTE

Build container to an image
```bash
docker-compose -f docker-compose.prod.yml build

docker images

// Run container on port 80 with the name react-app
docker run -p 80:80 --name react-app app-prod
```