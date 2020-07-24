# Fork

This repository was forked to allow executing typescript migrations and seeders during runtime without the need for compilation.

# sequelize/cli [![npm version](https://badge.fury.io/js/sequelize-cli.svg)](https://badge.fury.io/js/sequelize-cli) [![Build Status](https://travis-ci.org/sequelize/cli.svg?branch=master)](https://travis-ci.org/sequelize/cli) [![Greenkeeper badge](https://badges.greenkeeper.io/sequelize/cli.svg)](https://greenkeeper.io/)

The Sequelize Command Line Interface (CLI) _for TypeScript_

## Table of Contents
- [Installation](#installation)
- [Contributing](#contributing)
- [Documentation](#documentation)

## Installation

### Globally
Install CLI globally with

```bash
$ npm install -g sequelize-cli-typescript
```

Now you can run CLI using following command anywhere

```bash
$ sequelize
```

### Locally
Install CLI locally to your `node_modules` folder with

```bash
$ npm install --save sequelize-cli-typescript
```

You should be able to run CLI with

```bash
$ npx sequelize
```

### Differences from Sequelize-Cli _(non-TypeScript)_

With sequelize-cli, the ```model:generate``` command would produce _JavaScript_ files in two folders:
/models and /migrations, or other folders as specified in your .sequelizerc file.  The ```db:migrate```
command would then execute these _JavaScript_ files to update your database.

With sequelize-cli-typescript, ```model:generate``` produces _TypeScript_ files in the same two folders
(or again, as specified in your .sequelizerc file).  The ```db:migrate```
command would then execute these _TypeScript_ files to update your database.


### Usage
```
Sequelize CLI [Node: 6.11.2, CLI: 3.0.0, ORM: 4.8.0]

Commands:
  db:migrate                        Run pending migrations                      [aliases: db:migrate:up]
  db:migrate:schema:timestamps:add  Update migration table to have timestamps
  db:migrate:status                 List the status of all migrations
  db:migrate:undo                   Reverts a migration                         [aliases: db:migrate:down]
  db:migrate:undo:all               Revert all migrations ran
  db:seed                           Run specified seeder
  db:seed:undo                      Deletes data from the database
  db:seed:all                       Run every seeder
  db:seed:undo:all                  Deletes data from the database
  db:create                         Create database specified by configuration
  db:drop                           Drop database specified by configuration
  init                              Initializes project
  init:config                       Initializes configuration
  init:migrations                   Initializes migrations
  init:models                       Initializes models
  init:seeders                      Initializes seeders
  migration:generate                Generates a new migration file              [aliases: migration:create]
  model:generate                    Generates a model and its migration         [aliases: model:create]
  seed:generate                     Generates a new seed file                   [aliases: seed:create]

Options:
  --version  Show version number                                                [boolean]
  --help     Show help                                                          [boolean]
```

## Contributing

Sequelize CLI is always looking for contributions. You can help us with fixing bugs, reporting bugs or improving documentation.

Please read [contributing documentation](CONTRIBUTING.md)

## Documentation

- [Migrations Documentation](http://docs.sequelizejs.com/manual/tutorial/migrations.html)
- [CLI Options](docs/README.md)
- [Frequently Asked Questions](docs/FAQ.md)
