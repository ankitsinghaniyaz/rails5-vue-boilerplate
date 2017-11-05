# Rails + Vue Scaffold

This scaffold is supposed to quick iteration on new ideas. Here are some of the key choices made in making this.

- No CoffeeScript
- No Turbolink, I tried using it, it's a pain
- Webpack via Webpacker
- Vue.js
- Postgresql
- RSpec


## TODO

- Devise
- Active Admin
- iView CSS framework

## Setting up the Database

This is the most tricky part when setting up the application. You will need to make sure that `postgresql` is installed on your system. Here is how you can install it on Ubuntu:

```bash
# install postgres and required libs
sudo apt install postgresql postgresql-contrib libpq-dev
# create a new user and specify in database.yml
sudo -u postgres createuser -s {username}
# get into the psql prompt to do some work
sudo -u postgres psql
# setup password for the user
\password {username}
# when prompted enter a password and update the database.yml for the same
# then quit
\q

```

Things to do before moving into production:

- Make sure to change the database name to match your application name, not a bigdeal but makes a difference.

