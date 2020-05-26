# Lando Seed DB - Postgres

Lando Seed DB - Postgres is a starter project for a [Lando](https://lando.dev)-based development
environment. My main goal is to provide a useful function right out of the
box: as soon as you run `lando start` the first time, you will get a
containerized PostgreSQL development environment, capable of importing data from
dumps of other databases (like, say your production data). This supports the
use case of experimenting with writing potentially destructive queries for
your production data, all from the comfort of your own computer.

A secondary goal is to provide a starting place from which you can build
a more elaborate Lando development environment. Once you get familiar with
the database functionality, you can add an appserver to use this local data.

## Installation

You'll need to have [Docker](https://www.docker.com/products/docker-desktop)
installed, as well as [Lando](https://lando.dev/download/). Lando comes with
Docker Desktop, but you may already have Docker Desktop installed, which is
fine, just be sure that the version of Docker you have installed is at least
as current as the version that Lando wants to install.

## Usage

Clone/check out this project, then run `lando start` from the root
directory of this project.

Try some of these other commands:
* `lando psql` Run Arbritrary PostgreSQL commands via the CLI for PostgreSQL.
* `lando db-import <file>`  Import a dump file into the database.
* `lando` Show all availble Lando commands.

## What's Next?

That's kinda up to you.  If you have an SQL client you like (I'm partial to [TablePlus](https://www.tableplus.io/download) myself), fire it up and point it at `localhost:5432`

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## Credits

Thanks and credit are due to the creators of Lando, this project would not exist without them.

## License

[MIT](LICENSE.md)
