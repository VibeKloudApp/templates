# AngularJS + Node.js + Firestore (Cloud Run ready)

This project now serves a real **AngularJS (1.x)** front end from `public/index.html`.

## Features

- AngularJS module + controller (`vkApp` / `ProductController`)
- Product list fetch from `GET /api/products`
- Product creation form using `POST /api/products`
- Node.js + Express backend
- Dockerfile ready for Cloud Run (`PORT=8080`, `npm start`)

## Run locally

```bash
npm install
npm run dev
```

## Build and run container

```bash
docker build -t angularjs-nodejs .
docker run -p 8080:8080 angularjs-nodejs
```

If running outside GCP IAM, set `FIREBASE_SERVICE_ACCOUNT_KEY`.
