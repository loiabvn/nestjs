# NestJS Basic

[![NestJS](https://img.shields.io/badge/AmbitionVN-NestJS-red)](https://github.com/loiabvn/nestjs)

> Basic  


## Getting started

```bash
# 1. Clone the repository or click on "Use this template" button.
npx degit loiabvn/nestjs my-nest

# 2. Enter your newly-cloned folder.
cd my-nest

# 3. Create Environment variables file.
cp .env.dev .env

# 3. Install dependencies. (Make sure yarn is installed: https://yarnpkg.com/lang/en/docs/install)
yarn install
```


### Development
```bash
# 4. Run database + redis
docker-compose up -d

# 5. Run development server and open http://localhost:3000
yarn start:dev

# Launch the dev server with file watcher (optional)
yarn watch:dev

# Launch the dev server and enable remote debugger with file watcher (optional)
yarn debug:dev
```

### Build

To build the App, run

```bash
yarn build:prod
```

And you will see the generated file in `dist` that ready to be served.


### Migration
Some helper script to work with database

```bash
# To create new migration file
yarn migration:create migration_name

# Truncate full database (note: it isn't deleting the database)
yarn schema:drop

# Generate migration from update of entities
yarn migration:generate migration_name
```

### Generators
This project includes generators to speed up common development tasks. Commands include:

Note: Make sure you already have the nest-cli globally installed

```bash
# Install nest-cli globally
yarn global add @nestjs/cli

# Generate a new service
nest generate service users

# Generate a new class
nest g class users
```

## Features

When you use this template, try follow the checklist to update your info properly

- [x] Environment Configuration
- [x] Authentication + Roles
- [x] Log
- [x] Multi-languages
- [x] Swagger Api Documentation
- [x] Eslint

