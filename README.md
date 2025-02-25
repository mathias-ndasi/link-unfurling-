# link-unfurling

> Link Unfurling is the process of performing an action based on the hyperlink pasted into a message. This is implemented with NodeJs and Prisma. This is an ITV test from Ejara

> To run this repository on your local machine, follow the instructions below.

## Install and configure Mysql Server

1. Run the command below to install mysql server.

```bash
  $ sudo apt update
  $ sudo apt install mysql-server
```

2.  Configure mysql

```bash
 $ sudo mysql_secure_installation
```

3. For further configurations, follow this link: [setup and configure mysql on ubuntu](https://www.digitalocean.com/community/tutorials/how-to-install-mysql-on-ubuntu-20-04)
4. Create a database schema with name '**link-unfurling**'

## Setup Custom Environment file [.env]

1. Run the command below to create your local customer environment file.

```bash
  $ cp -b .env.example .env
```

2. Edit your environment file with your corresponding mysql db url string.

## Update the database schema with migrations

### Generate prisma client

```bash
  $ npx prisma generate
```

### Apply migrations

```bash
  $ npx prisma migrate dev
```

### Reset your database and apply all migrations

```bash
  $ npx prisma migrate reset
```

### Apply pending migrations to the database

```bash
  $ npx prisma migrate deploy
```

### Check the status of migrations

```bash
  $ npx prisma migrate status
```

[Nest](https://github.com/nestjs/nest) framework TypeScript starter repository.

<p  align="center">  <a  href="http://nestjs.com/"  target="blank"><img  src="https://nestjs.com/img/logo_text.svg"  width="320"  alt="Nest Logo" /></a> </p>

[circleci-image]: https://img.shields.io/circleci/build/github/nestjs/nest/master?token=abc123def456
[circleci-url]: https://circleci.com/gh/nestjs/nest

<p  align="center">A progressive <a  href="http://nodejs.org"  target="_blank">Node.js</a> framework for building efficient and scalable server-side applications.</p>

<p  align="center"> <a  href="https://www.npmjs.com/~nestjscore"  target="_blank"><img  src="https://img.shields.io/npm/v/@nestjs/core.svg"  alt="NPM Version" /></a> <a  href="https://www.npmjs.com/~nestjscore"  target="_blank"><img  src="https://img.shields.io/npm/l/@nestjs/core.svg"  alt="Package License" /></a> <a  href="https://www.npmjs.com/~nestjscore"  target="_blank"><img  src="https://img.shields.io/npm/dm/@nestjs/common.svg"  alt="NPM Downloads" /></a> <a  href="https://circleci.com/gh/nestjs/nest"  target="_blank"><img  src="https://img.shields.io/circleci/build/github/nestjs/nest/master"  alt="CircleCI" /></a> <a  href="https://coveralls.io/github/nestjs/nest?branch=master"  target="_blank"><img  src="https://coveralls.io/repos/github/nestjs/nest/badge.svg?branch=master#9"  alt="Coverage" /></a> <a  href="https://discord.gg/G7Qnnhy"  target="_blank"><img  src="https://img.shields.io/badge/discord-online-brightgreen.svg"  alt="Discord"/></a> <a  href="https://opencollective.com/nest#backer"  target="_blank"><img  src="https://opencollective.com/nest/backers/badge.svg"  alt="Backers on Open Collective" /></a> <a  href="https://opencollective.com/nest#sponsor"  target="_blank"><img  src="https://opencollective.com/nest/sponsors/badge.svg"  alt="Sponsors on Open Collective" /></a> <a  href="https://paypal.me/kamilmysliwiec"  target="_blank"><img  src="https://img.shields.io/badge/Donate-PayPal-ff3f59.svg"/></a> <a  href="https://opencollective.com/nest#sponsor"  target="_blank"><img  src="https://img.shields.io/badge/Support%20us-Open%20Collective-41B883.svg"  alt="Support us"></a> <a  href="https://twitter.com/nestframework"  target="_blank"><img  src="https://img.shields.io/twitter/follow/nestframework.svg?style=social&label=Follow"></a>
</p>

<!--[![Backers on Open Collective](https://opencollective.com/nest/backers/badge.svg)](https://opencollective.com/nest#backer)



[![Sponsors on Open Collective](https://opencollective.com/nest/sponsors/badge.svg)](https://opencollective.com/nest#sponsor)-->

## Description

[Nest](https://github.com/nestjs/nest) framework TypeScript starter repository.

## Installation

```bash
$ npm install
```

## Running the app

```bash
# development
$ npm run start

# watch mode
$ npm run start:dev

# production mode
$ npm run start:prod
```

## Test

```bash
# unit tests
$ npm run test

# e2e tests
$ npm run test:e2e

# test coverage
$ npm run test:cov

```

## OpenAPI [Swagger]

Route to [http://localhost:3000/api/](http://localhost:3000/api/) to test the available route with [Swagger](https://docs.nestjs.com/openapi/introduction).

## Support

Nest is an MIT-licensed open source project. It can grow thanks to the sponsors and support by the amazing backers. If you'd like to join them, please [read more here](https://docs.nestjs.com/support).

## Stay in touch

- Author - [Kamil Myśliwiec](https://kamilmysliwiec.com)

- Website - [https://nestjs.com](https://nestjs.com/)

- Twitter - [@nestframework](https://twitter.com/nestframework)

## License

Nest is [MIT licensed](LICENSE).
