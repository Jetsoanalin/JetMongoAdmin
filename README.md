<<<<<<< HEAD
# adminMongo
=======
# JetMongoAdmin
>>>>>>> a5e51190eaad7377e704f1400b0b9a5a39d252c1

![npm downloads badge](https://img.shields.io/npm/dm/admin-mongo.svg "npm download badge")
![npm version badge](https://img.shields.io/npm/v/admin-mongo.svg "npm version badge")
[![Build Status](https://travis-ci.org/mrvautin/adminMongo.svg?branch=master)](https://travis-ci.org/mrvautin/adminMongo)
<<<<<<< HEAD
[![Github stars](https://img.shields.io/github/stars/mrvautin/adminMongo.svg?style=social&label=Star)](https://github.com/mrvautin/adminMongo)

adminMongo is a cross platform user interface (GUI) to handle all your MongoDB connections/databases needs. adminMongo is fully responsive and should work on a range of devices.

> adminMongo connection information (including username/password) is stored unencrypted in a config file, it is not recommended to run this application on a production or public facing server without proper security considerations.

## Support

If my work helps you, please consider [![buying me a coffee](https://cdn-images-1.medium.com/max/738/1*G95uyokAH4JC5Ppvx4LmoQ@2x.png)](https://www.buymeacoffee.com/mrvautin)

## Installation

1. Navigate to folder & install adminMongo: `git clone https://github.com/mrvautin/adminMongo.git && cd adminMongo`
=======


## Disclaimer : This is a Forked project which is modified according to my need (ReBuilding under MIT License *

JetMongoAdmin is a cross platform user interface (GUI) to handle all your MongoDB connections/databases needs. JetMongoAdmin is fully responsive and should work on a range of devices.

> JetMongoAdmin connection information (including username/password) is stored unencrypted in a config file, it is not recommended to run this application on a production or public facing server without proper security considerations.


## Installation

1. Navigate to folder & install JetMongoAdmin: `git clone https://github.com/jetsoanalin/JetMongoAdmin.git && cd JetMongoAdmin`
>>>>>>> a5e51190eaad7377e704f1400b0b9a5a39d252c1
2. Install dependencies: `npm install`
3. Start application: `npm start` or `node app`
4. Visit [http://127.0.0.1:1234](http://127.0.0.1:1234) in your browser

> Note: Node.js version 4.x or above is required

## Electron App

<<<<<<< HEAD
adminMongo can also be used as a cross platform Electron application. Due to the size of Electron it will need to be built manually.
=======
JetMongoAdmin can also be used as a cross platform Electron application. Due to the size of Electron it will need to be built manually.
>>>>>>> a5e51190eaad7377e704f1400b0b9a5a39d252c1

To build for Mac:

`$ npm run-script packageOsx`

To build for Windows:

`$ npm run-script packageWin32`

To build for Linux:

`$ npm run-script packageLinux`

Once built, the executable will be in the `/releases` folder.

<<<<<<< HEAD
### Prebuilt binaries

Prebuilt binaries can be downloaded here:

[Mac 64bit](https://github.com/mrvautin/adminMongo/releases/download/1.0.0/adminMongo_Mac.zip)

[Windows 32bit](https://github.com/mrvautin/adminMongo/releases/download/1.0.0/adminMongo_Win32.zip)

[Windows 64bit](https://github.com/mrvautin/adminMongo/releases/download/1.0.0/adminMongo_Win64.zip)

> The Electron builds have been tested on Mac and Windows 10. Linux has not been tested. Please report any issues.

=======
>>>>>>> a5e51190eaad7377e704f1400b0b9a5a39d252c1
## Deploy on Heroku

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/mrvautin/adminMongo)

<<<<<<< HEAD
## Demo (read only)

A read only demo can be seen [here](http://demo.adminmongo.markmoffat.com)
=======
>>>>>>> a5e51190eaad7377e704f1400b0b9a5a39d252c1

## Features

* Manage from a connection level for easy access to multiple databases
* Create/Delete databases
* Backup/Restore databases
* Create/Delete/Edit collection
* Create/Delete/Edit documents
* Create/Delete indexes
* Query documents
* Collection statistics
* Export collections in JSON format
* Server monitoring

### Current limitations

* Documents need to have an "_id" value which is a string, integer, or MongoDB ObjectId. Documents using Composite ID indexing is currently not supported.
* Connection strings with multiple hosts for replica sets are currently not supported.

## Configuration

<<<<<<< HEAD
adminMongo will listen on host: `localhost` and  port: `1234` by default. This can be overwritten by adding a config file in `/config/app.json`. For example:
=======
JetMongoAdmin will listen on host: `localhost` and  port: `1234` by default. This can be overwritten by adding a config file in `/config/app.json`. For example:
>>>>>>> a5e51190eaad7377e704f1400b0b9a5a39d252c1

```
{
    "app": {
        "host": "10.0.0.1",
        "port": 4321,
        "password": "secureadminpassword",
        "locale": "de",
        "context": "dbApp",
        "monitoring": false
    }
}
```

> Note: Any changes to the config file requires a restart of the application

<<<<<<< HEAD
All above parameters are usable through the environment which makes it very handy to when using adminMongo as a docker container!
=======
All above parameters are usable through the environment which makes it very handy to when using JetMongoAdmin as a docker container!
>>>>>>> a5e51190eaad7377e704f1400b0b9a5a39d252c1
just run `docker run -e HOST=yourchoice -e PORT=1234 ...`

The config file (optional) options are:

|Option|Env-variable|Definition|
|--- |--- |--- |
<<<<<<< HEAD
|`host`|`HOST`|The IP address  `adminMongo`  will listen on|
|`port`|`PORT`|The Port `adminMongo` will listen on|
|`password`|`PASSWORD`|An application level password to add simply authentication|
|`locale`|`LOCALE`|The locale is automatically set to the detected locale of Nodejs. If there is not a translation, `adminMongo` will default to English. This setting overrides the default/detected value|
|`context`|`CONTEXT`|Setting a `context` of "dbApp" is like changing the base URL of the app and will mean the app will listen on `http://10.0.0.1:4321/dbApp`. Ommiting a context will mean the application will listen on root. Eg: `http://10.0.0.1:4321`. This setting can be useful when running `adminMongo` behind Nginx etc.|
=======
|`host`|`HOST`|The IP address  `JetMongoAdmin`  will listen on|
|`port`|`PORT`|The Port `JetMongoAdmin` will listen on|
|`password`|`PASSWORD`|An application level password to add simply authentication|
|`locale`|`LOCALE`|The locale is automatically set to the detected locale of Nodejs. If there is not a translation, `JetMongoAdmin` will default to English. This setting overrides the default/detected value|
|`context`|`CONTEXT`|Setting a `context` of "dbApp" is like changing the base URL of the app and will mean the app will listen on `http://10.0.0.1:4321/dbApp`. Ommiting a context will mean the application will listen on root. Eg: `http://10.0.0.1:4321`. This setting can be useful when running `JetMongoAdmin` behind Nginx etc.|
>>>>>>> a5e51190eaad7377e704f1400b0b9a5a39d252c1
|`monitoring`|`MONITORING`|Whether to run monitoring at regular intervals. Defaults to true or on|

### Setting a context path

Setting a `context` of "dbApp" is like changing the base URL of the app and will mean the app will listen on `http://10.0.0.1:4321/dbApp`. Ommiting a context will mean the application will listen on
<<<<<<< HEAD
root. Eg: `http://10.0.0.1:4321`. This setting can be useful when running `adminMongo` behind Nginx etc.
=======
root. Eg: `http://10.0.0.1:4321`. This setting can be useful when running `JetMongoAdmin` behind Nginx etc.
>>>>>>> a5e51190eaad7377e704f1400b0b9a5a39d252c1

An example Nginx server block. Note the `location /dbApp {` and `proxy_pass http://10.0.0.1:4321/dbApp;` lines match
the `context` set in the `/config/app.json` file.

```
server {
    listen 80;

    server_name mydomain.com www.mydomain.com;

    location /dbApp {
        proxy_pass http://10.0.0.1:4321/dbApp;
        proxy_http_version 1.1;
        proxy_set_header Upgrade $http_upgrade;
        proxy_set_header Connection 'upgrade';
        proxy_set_header Host $host;
        proxy_cache_bypass $http_upgrade;
    }
}
```

### Language locale

> Looking for people to translate into other languages. If you can help, grab the `/locale/en.js` file, translate to your language and submit a pull request.

<<<<<<< HEAD
The locale is automatically set to the detected locale of Nodejs. If there is not a translation, `adminMongo` will default to English. To override the detected locale
=======
The locale is automatically set to the detected locale of Nodejs. If there is not a translation, `JetMongoAdmin` will default to English. To override the detected locale
>>>>>>> a5e51190eaad7377e704f1400b0b9a5a39d252c1
a setting can be added to the `app.json` file. See Configuration section for a "German" example.

### Authentication

<<<<<<< HEAD
By default `adminMongo` is not password protected. You can add password authentication by adding a `password` value to the `/config/app.json` file
(See the Configuration section). Once added you will need to restart `adminMongo` and all routes will be protected until the correct password is added. You
=======
By default `JetMongoAdmin` is not password protected. You can add password authentication by adding a `password` value to the `/config/app.json` file
(See the Configuration section). Once added you will need to restart `JetMongoAdmin` and all routes will be protected until the correct password is added. You
>>>>>>> a5e51190eaad7377e704f1400b0b9a5a39d252c1
will then be authenticated for the life of the session (60 mins by default) or if the "Logout" link is clicked.

## Usage

### Create a connection

<<<<<<< HEAD
After visiting [http://127.0.0.1:1234](http://127.0.0.1:1234) you will be presented with a connection screen. You need to give your connection a unique name as a reference when using adminMongo and a MongoDB formatted connection string. The format of a MongoDB connection string can form: `mongodb://<user>:<password>@127.0.0.1:<port>/<db>` where specifying to the `<db>` level is optional. For more information on MongoDB connection strings, see the [official MongoDB documentation](http://docs.mongodb.org/manual/reference/connection-string/).
=======
After visiting [http://127.0.0.1:1234](http://127.0.0.1:1234) you will be presented with a connection screen. You need to give your connection a unique name as a reference when using JetMongoAdmin and a MongoDB formatted connection string. The format of a MongoDB connection string can form: `mongodb://<user>:<password>@127.0.0.1:<port>/<db>` where specifying to the `<db>` level is optional. For more information on MongoDB connection strings, see the [official MongoDB documentation](http://docs.mongodb.org/manual/reference/connection-string/).
>>>>>>> a5e51190eaad7377e704f1400b0b9a5a39d252c1

You can supply a connection options object (see [docs](http://mongodb.github.io/node-mongodb-native/2.1/reference/connecting/connection-settings/)) with each connection.

For example:

```
{
    "poolSize": 10,
    "autoReconnect": false,
    "ssl": false
}
```

Note: The connection can be either local or remote hosted on VPS or MongoDB service such as mLab.

The connection can also be automatically initiated through the environment (or with the docker -e parameters)

|Env-variable|Description|
|--- |--- |
|`CONN_NAME`|The name of the connection to create on boot|
|`DB_USERNAME`|The username for the database connection|
|`DB_PASSWORD`|The password for the database user|
|`DB_HOST`|The host IP address or DNS name without the port!|
|`DB_PORT`|The port of the mongoDB database, if not provided the default 27017 will be used|
|`DB_NAME`|The name of the database|

*The Connection setup screen*
<<<<<<< HEAD
![adminMongo connections screen](https://raw.githubusercontent.com/mrvautin/mrvautin.github.io/master/images/adminMongo/adminMongo_connections.png "adminMongo connections screen")
=======
![JetMongoAdmin connections screen](https://raw.githubusercontent.com/mrvautin/mrvautin.github.io/master/images/adminMongo/adminMongo_connections.png "JetMongoAdmin connections screen")
>>>>>>> a5e51190eaad7377e704f1400b0b9a5a39d252c1

### Connection/Database admin

After opening your newly created connection, you are able to see all database objects associated with your connection. Here you can create/delete collections, create/delete users and see various stats for your database.

*The connections/database screen*
<<<<<<< HEAD
![adminMongo database screen](https://raw.githubusercontent.com/mrvautin/mrvautin.github.io/master/images/adminMongo/adminMongo_dbview.png "adminMongo database screen")
=======
![JetMongoAdmin database screen](https://raw.githubusercontent.com/mrvautin/mrvautin.github.io/master/images/adminMongo/adminMongo_dbview.png "JetMongoAdmin database screen")
>>>>>>> a5e51190eaad7377e704f1400b0b9a5a39d252c1

### Collections

After selecting your collection from the "Database Objects" menu, you will be presented with the collections screen. Here you can see documents in pagination form, create new documents, search documents, delete, edit documents and view/add indexes to your collection.

*The collections screen*
<<<<<<< HEAD
![adminMongo collections screen](https://raw.githubusercontent.com/mrvautin/mrvautin.github.io/master/images/adminMongo/adminMongo_collectionview.png "adminMongo collections screen")
=======
![JetMongoAdmin collections screen](https://raw.githubusercontent.com/mrvautin/mrvautin.github.io/master/images/adminMongo/adminMongo_collectionview.png "JetMongoAdmin collections screen")
>>>>>>> a5e51190eaad7377e704f1400b0b9a5a39d252c1

### Searching/Querying documents

You can perform searches of documents using the `Search documents` button on the collections screen. You will need to enter the key (field name) and value. Eg: key = "_id" and value = "569ff81e0077663d78a114ce" (Only works on string "_id" fields - Use "Query Documents" for ObjectID's).

> You can clear your search by clicking the `Reset` button on the collections screen.

*Simple search documents*
<<<<<<< HEAD
![adminMongo search documents](https://raw.githubusercontent.com/mrvautin/mrvautin.github.io/master/images/adminMongo/adminMongo_searchdocuments.png "adminMongo search documents")
=======
![JetMongoAdmin search documents](https://raw.githubusercontent.com/mrvautin/mrvautin.github.io/master/images/adminMongo/adminMongo_searchdocuments.png "JetMongoAdmin search documents")
>>>>>>> a5e51190eaad7377e704f1400b0b9a5a39d252c1

Complex querying of documents is done through the "Query documents" button. This allows a query Object to be passed to MongoDB to return results.
Queries can be written in full BSON format or EJSON format. For example these queries should return the same results:

```
{
    ObjectId("56a97ed3f718fe9a4f599489")
}
```

is equivalent to:

```
{
    "$oid": "56a97ed3f718fe9a4f599489"
}
```

*Query documents*
<<<<<<< HEAD
![adminMongo search documents](https://raw.githubusercontent.com/mrvautin/mrvautin.github.io/master/images/adminMongo/adminMongo_querydocuments.png "adminMongo search documents")
=======
![JetMongoAdmin search documents](https://raw.githubusercontent.com/mrvautin/mrvautin.github.io/master/images/adminMongo/adminMongo_querydocuments.png "JetMongoAdmin search documents")
>>>>>>> a5e51190eaad7377e704f1400b0b9a5a39d252c1


### Documents

Adding and editing documents is done using a JSON syntax highlighting control.

*Editing a document*
<<<<<<< HEAD
![adminMongo documents](https://raw.githubusercontent.com/mrvautin/mrvautin.github.io/master/images/adminMongo/adminMongo_docedit.png "adminMongo documents")
=======
![JetMongoAdmin documents](https://raw.githubusercontent.com/mrvautin/mrvautin.github.io/master/images/adminMongo/adminMongo_docedit.png "JetMongoAdmin documents")
>>>>>>> a5e51190eaad7377e704f1400b0b9a5a39d252c1

Documents with Media embedded show previews

*Documents with media*
<<<<<<< HEAD
![adminMongo media](https://raw.githubusercontent.com/mrvautin/mrvautin.github.io/master/images/adminMongo/adminMongo_media.png "adminMongo media documents")
=======
![JetMongoAdmin media](https://raw.githubusercontent.com/mrvautin/mrvautin.github.io/master/images/adminMongo/adminMongo_media.png "JetMongoAdmin media documents")
>>>>>>> a5e51190eaad7377e704f1400b0b9a5a39d252c1

### Server Monitoring

*Functionality currently in Beta*

Selected server monitoring is done at regular intervals and stored in local database store for 24hrs.

*New connections require an app restart for monitoring to commence*

*Server monitoring*
<<<<<<< HEAD
![adminMongo server monitoring](https://raw.githubusercontent.com/mrvautin/mrvautin.github.io/master/images/adminMongo/adminMongo_servermonitoring.png "adminMongo server monitoring")
=======
![JetMongoAdmin server monitoring](https://raw.githubusercontent.com/mrvautin/mrvautin.github.io/master/images/adminMongo/adminMongo_servermonitoring.png "JetMongoAdmin server monitoring")
>>>>>>> a5e51190eaad7377e704f1400b0b9a5a39d252c1

### Indexes

Indexes can be added from the collection screen. Please see the [official MongoDB documentation](https://docs.mongodb.org/manual/indexes/) on adding indexes.

*Viewing/Adding indexes*
<<<<<<< HEAD
![adminMongo documents](https://raw.githubusercontent.com/mrvautin/mrvautin.github.io/master/images/adminMongo/adminMongo_manageindexes.png "adminMongo indexes")

## Tests

The `adminMongo` API tests include:
=======
![JetMongoAdmin documents](https://raw.githubusercontent.com/mrvautin/mrvautin.github.io/master/images/adminMongo/adminMongo_manageindexes.png "JetMongoAdmin indexes")

## Tests

The `JetMongoAdmin` API tests include:
>>>>>>> a5e51190eaad7377e704f1400b0b9a5a39d252c1

- Add and remove a connection
- Add and remove a database
- Add, remove and rename a collection
- Create and delete a user
- Add, query and delete a document

To run tests, simply run:

```
npm test
```

**Note: You will need to ensure there is no password protection setup in the `/config/app.json`.**

*You may need to edit the variables and connection string in `/tests/tests.js` for your MongoDB instance.*

If you see any missing tests, please submit a PR.

<<<<<<< HEAD
## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## Future plans

Please make any suggestions.

## License

[The MIT License](https://github.com/mrvautin/adminMongo/tree/master/LICENSE)
=======
## Feature Upgradation after Fork from user @mrvautin plans

Working on upgradation

## License

[The MIT License](https://github.com/jetsoanalin/JetMongoAdmin/tree/master/LICENSE)
>>>>>>> a5e51190eaad7377e704f1400b0b9a5a39d252c1
