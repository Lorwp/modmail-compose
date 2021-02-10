# Modmail Stack

A stack version of [kyb3r/modmail](https://github.com/kyb3r/modmail/) with dependencies.

## Installation

First, make a bot for the application per the instructions on the [Main Modmail Repo](https://github.com/kyb3r/modmail/wiki/Installation)

Then clone locally and create `.env` with the following contents:

```bash
MONGO_INITDB_ROOT_USERNAME=root
MONGO_INITDB_ROOT_PASSWORD=yourpassword
TOKEN= #your discord bot token
DATABASE_TYPE=mongodb
GUILD_ID= #Your Server ID
OWNERS= #Your User ID
LOG_URL= # The External url of logviewer
CONNECTION_URL=mongodb+srv://Username:MyPassword@mongodb/ # per URI, replace username and mypassword with connection details to the db. Can also replace with an external db
```

By default logviewer is accessible at 127.0.0.1:8000, you probably want to put this behind a reverse proxy like [caddy](https://registry.hub.docker.com/_/caddy)


Then run `docker-compose up -d` to bring it up, then continue past step 5.11 of the [Main Guide](https://github.com/kyb3r/modmail/wiki/Installation-(cont.)#6-modmail)
