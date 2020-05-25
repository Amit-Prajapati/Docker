## Running Locally - Development Mode
```
yarn install && npm install
docker build -t <appName>:dev 
docker-compose up -d --build
```

## Stopping Locally - Development Mode
```
docker-compose stop
```
## Running on Server - Production Mode
Update URL Provided in Line No.10 of Dockerfile.prod to the latest NLB URL before running the following commands.

```
yarn install && npm install
docker-compose -f docker-compose.prod.yml up -d --build
```
