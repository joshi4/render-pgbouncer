PgBouncer
=========

[![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy)

### Usage

Fork this repo and use the `Deploy to Render` button to launch `pgbouncer` as a private service in your Render account.

The dashboard will prompt you to set a value for the `DATABASE_URL` environment variable. Set the value to be the `Internal Connection String` of the Render database you wish to connect to.

You will also need to make the following changes to your app:

* Update your app to use the hostname of the private service created above instead of the db hostname.
* Update your connection string to use `sslmode=disable`
