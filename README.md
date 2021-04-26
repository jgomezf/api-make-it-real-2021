# Node APIRest

## Prerequisites

- [Node](https://nodejs.org/)
- NPM, built into Node
- [yarn](https://yarnpkg.com/getting-started/install)
- [MongoDB](https://www.mongodb.com/try/download/community) or [MondoDB Atlas](https://www.mongodb.com/cloud/atlas2)
- [Postman](https://www.postman.com/) or [Insomnia](https://insomnia.rest/) or any client api rest.

## Before starting

Make sure you have yarn installed, run on console.

```bash
yarn --version
```

if it return an error, please install [yarn](https://yarnpkg.com/getting-started/install).

```
npm install -g yarn
```

## Clone the repo

```bash
git clone https://github.com/jestrade/api-make-it-real-2021.git
```

## Enter to folder project

```bash
cd api-make-it-real-2021
```

## Install the app

```bash
yarn
```

## Create .env file

- Configuration Example:
  - HTTP_HOST -> IP of server, default is 127.0.0.1.
  - HTTP_PORT -> Node listening port, default is 3000.
  - LOG_ACCESS -> Path where the logs will be stored.
  - JWTKEY -> Is used by [JWT](https://www.npmjs.com/package/jsonwebtoken) to sign the token.
  - APIWEATHERKEY -> Is used to consume the [API](https://openweathermap.org/api).
  - DB_CONNECTION_STRING -> Connection string to connect [mongodb](https://mongoosejs.com/docs/connections.html) database
  - SALT_ROUNDS -> Controls how much time is needed to calculate a single BCrypt hash, default is 10.

Example connection string local, more info. [MongoDB](https://www.mongodb.com/try/download/community).

```bash
mongodb://username:password@host:port/database
```

Example connection string in cloud, more info [MondoDB Atlas](https://www.mongodb.com/cloud/atlas2).

```bash
mongodb+srv://<username>:<password>@cluster0.rwp0b.mongodb.net/myFirstDatabase?retryWrites=true&w=majority
```

```bash
HTTP_HOST=127.0.0.1
HTTP_PORT=3000
LOG_ACCESS=../logs/access.log
JWTKEY=my-secret-key
APIWEATHERKEY=
DB_CONNECTION_STRING=
SALT_ROUNDS=10
```

## Install nodemon as development dependency

```bash
yarn add -D nodemon
```

## Run the app

### Without nodemon

Run project without nodemon

```bash
yarn start
```

### With nodemon

Run project without nodemon

```bash
yarn run dev
```

### Run tests

```bash
yarn run test
```
