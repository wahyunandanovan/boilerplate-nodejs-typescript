
# Boilerplate Nodejs TypeScript 


Tujuan utama dari repositori ini adalah untuk menunjukkan pengaturan proyek dan alur kerja end-to-end yang baik untuk menulis kode Mongoose,Node.js dan Express dalam TypeScript .lengkap dengan middleware, model, route, dan tipe.

Contoh ini dilengkapi dengan REST API yang lengkap. untuk menangani fitur Authentifikasi dan CRUD.

## Teknologi

**Server:** Node, Express, typescript, ts-node

**DataBase:** mongoose


## Jalankan di lokal

Clone project

```bash
  git clone https://github.com/wahyunandanovan/node-typescript.git
```

Pergi ke project direktori

```bash
  cd node-typescript
```

Instal dependency

```bash
  npm install
```

Start tsc

```bash
  npm run watch
```

Start server

```bash
  npm run dev
```


## Environment Variables

Untuk menjalankan proyek ini, Anda perlu menambahkan variabel lingkungan berikut ke file .env Anda
`NODE_ENV="production"`, 
`NODE_ENV="local"`, 
`MONGO_DB_USER`, 
`MONGO_DB_PASSWORD`. 
`JWT_SECRETS`, 
`SMTP_HOST`, 
`SMTP_PORT`, 
`SMTP_USERNAME`, 
`SMTP_PASSWORD`, 
`SMTP_SENDER`,

> **Note!** Pastikan Anda sudah membuat aplikasi menggunakan npm run start

## Refrensi API 

#### Create user

```http
  POST /api/v1/user/sign-up
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `firstName`      | `string` | **Required**. Your API key |
| `lastName`      | `string` | **Required**. Your API key |
| `avatar`      | `string` | **Required**. Your API key |
| `email`      | `string` | **Required**. Your API key |
| `password`      | `string` | **Required**. Your API key |
| `confirmPassword`      | `number` | **Required**. Your API key |

#### login user

```http
  POST /api/v1/auth/login
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `email`      | `number` | **Required**. Your API key |
| `password`      | `string` | **Required**. Your API key |


#### Get all users

```http
  GET /api/v1/user/fetch
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `_id` | `uuid` | **Required**.API key |
| `firstName` | `string` | **Required**.API key |
| `lastName` | `string` | **Required**.API key |
| `gender` | `string` | **Required**.API key |
| `dateOfBirth` | `string` | **Required**.API key |
| `residence` | `string` | **Required**.API key |
| `avatar` | `string` | **Required**.API key |
| `email` | `string` | **Required**.API key |
| `password` | `string` | **Required**.API key |
| `role` | `string` | **Required**.API key |
| `isEmailVerified` | `boolean` | **Required**.API key |
| `isEmailVerified` | `boolean` | **Required**.API key |


