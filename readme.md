# Modmail Stack

A stack version of [kyb3r/modmail](https://github.com/kyb3r/modmail/) with dependencies.

## Installation

First, make a bot for the application per the instructions on the [Main Modmail Repo](https://github.com/kyb3r/modmail/wiki/Installation)

Then clone locally, create `.mongoenv`, `.env` and `.mongo_url` with the following contents:

`.mongoenv`:
```bash
# Details for the mongodb root user
MONGO_INITDB_ROOT_USERNAME=root
MONGO_INITDB_ROOT_PASSWORD=yourpassword
```
`.env`:
```bash
TOKEN= #your discord bot token
DATABASE_TYPE=mongodb
GUILD_ID= #Your Server ID
OWNERS= #Your User ID
LOG_URL= # The External url of logviewer
```
`.mongo_url`:
```bash
CONNECTION_URL=mongodb+srv://Username:MyPassword@mongodb/ # per URI, replace username and mypassword with connection details to the db. Can also replace with an external db
```

info about reverse proxy for the logviewer here idk


Then run `docker-compose up -d` to bring it up, then continue past step 5.11 of the [Main Guide](https://github.com/kyb3r/modmail/wiki/Installation-(cont.)#6-modmail)
