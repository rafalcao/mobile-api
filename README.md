# Mobile API - Serverless

## Node container
```bash
docker run -it -d --name="node" -v /var/www/html/mobile-api/:/var/www/html/mobile-api/ node:16.17
```

## Install Serverless
```bash
npm install -g serverless
```

## AWS Credentials
```bash
serverless config credentials -o -p aws -k AKIA3EQ2MB4GNCRBRX63 -s eVlXbLT6r7ASEgdzbpBR3fPXqD/QPMDv5XPahL+V
```

## Deploy
```bash
serverless deploy --verbose
```

## Destroy
```bash
serverless remove
```

## Local Test
```bash
serverless invoke local --function index
```