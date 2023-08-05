# Mongo-Mongo-Express Docker Compose

It contains docker instances for both **Mongo** & **Mongo Express** internally connected via bridge network.

## Mongo

Mongo, the database server itself can be accessed on host machine (localhost) on port _27017_.

### Description

Below configuration are already set by default via `mongoCreds.env` file and can be modified by overriding the same.

| Config   | Value | Comment                          |
| -------- | ----- | -------------------------------- |
| Port     | 27017 | Exposed at localhost (127.0.0.1) |
| Username | root  |                                  |
| Password | root  |                                  |

**Note**: The MONGODB_URL required to interact with MongoDB would be [mongodb://root:root@localhost:27017/db](mongodb://root:root@localhost:27017/db) where _db_ is the name of the database you will use.

## Mongo Express

Mongo Express is integrated to graphically visualize the mongo database.
It can be accessed on host machine (localhost) web browser at [http://localhost:8081](http://localhost:8081).

### Configuration

Below configuration are already set by default via `mongoExpressCreds.env` file and can be modified by overriding the same.

| Config   | Value | Comment                          |
| -------- | ----- | -------------------------------- |
| Port     | 8081  | Exposed at localhost (127.0.0.1) |
| Username | root  |                                  |
| Password | root  |                                  |