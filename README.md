# Google Maps Presenter
[![codecov](https://codecov.io/gh/vkaracic/cle-maps/branch/master/graph/badge.svg)](https://codecov.io/gh/vkaracic/cle-maps)

Custom Learning Experience with Google Maps.

# Installation
- create a new database and change the database related value in the configuration file
- run `npm install` to install all the needed packages
- run `npm run migrate` to create the database tables
- run `npm run compile_scss` to compile the SCSS to CSS
- add a session secret to your configuration file

At this point only getting the Google Maps API key is left. To do that go to the [Google developers page](https://developers.google.com/maps/documentation/javascript/get-api-key) and get or create a new API key. Set that key in your `config.json` file and you are good to go.

# Example settings
config.json:
```
{
  "development": {
    "username": "root",
    "password": "root",
    "database": "cle",
    "host": "localhost",
    "dialect": "mysql",
    "mapsApiKey": "your-google-maps-api-key",
    "sessionSecret": "top-secret"
  },
  "production": {
    "username": "root",
    "password": super-strong-password,
    "database": "database_production",
    "host": "production",
    "dialect": "mysql",
    "mapsApiKey": "your-google-maps-api-key",
    "sessionSecret": "top-secret"
  }
}
```

# Testing
You can run the tests with `npm run test`.
You can run the linter with `npm run lint`.

# Contribution
If you have a suggestion, question or found a bug, please [open an issue](https://github.com/vkaracic/cle-maps/issues/new) for it.

If you want to contribute code then please open a pull request with details about the changes that you propose.
