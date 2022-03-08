# ![RealWorld Example App](logo.png)

> ### Example Node.Js (Koa.js + Knex) codebase containing real world examples (CRUD, auth, advanced patterns, etc) that adheres to the [RealWorld](https://github.com/gothinkster/realworld-example-apps) spec and API.

This repo is functionality complete — PRs and issues welcome!

This codebase was created to demonstrate a fully fledged fullstack application built with **Koa.js + Knex** including CRUD operations, authentication, routing, pagination, and more.

We've gone to great lengths to adhere to the **Koa.js + Knex** community styleguides & best practices.

For more information on how to this works with other frontends/backends, head over to the [RealWorld](https://github.com/gothinkster/realworld) repo.

# Getting started

## Installation

1. Install [Node.JS](https://nodejs.org/en/download/package-manager/) previous version 13.14.0
2. Clone this repo
3. Install dependencies, just run in project folder: `npm i` or `yarn`

## Usage

1. Doing database migrations `npm run db:migrate`

2. Upload test data `npm run db:load`

3. run `npm run dev` to start server

4. In the frontend just change the API url to `const baseUrl = 'http://localhost:3000/api'`

## Testing

1. run `npm test` for tests

## Server Configuration (optional)

You can use `.env` file, to configure project like this:

```
NODE_ENV = development
PORT = 3000
SECRET = secret
DB_CLIENT = sqlite3
#DB_CONNECTION = postgres://user:password@localhost:5432/db_name
```

you can just copy `.example-env`

## Variables description

`NODE_ENV` - specify env: development/production/test. `development` by default

`NODE_PORT` - specify port: `3000` by default

`SECRET` - custom secret for generating passwords. `secret` by default

`DB_CLIENT` - database to use. `pg` - postgress or `sqlite3`. `sqlite3` by default

`DB_CONNECTION` - db connection string for `postgress` database.

## Fixtures (optional)

1. load fixtures: `npm run db:load` (it uses settings from `.env`). Don't forget to set `NODE_ENV`.

## Styleguide

[![Standard - JavaScript Style Guide](https://cdn.rawgit.com/feross/standard/master/badge.svg)](https://github.com/feross/standard)

# How it works

> Describe the general architecture of your app here
