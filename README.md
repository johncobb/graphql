# Learning GraphQL

## Table of contents
- [Learning GraphQL](#learning-graphql)
  - [Table of contents](#table-of-contents)
  - [Prerequisites:](#prerequisites)
  - [Examples:](#examples)
      - [Download MongoDB from website](#download-mongodb-from-website)
      - [Extract MongoDB](#extract-mongodb)
      - [Setup directory/permissions where MongoDB will store files](#setup-directorypermissions-where-mongodb-will-store-files)
      - [Running Mongo daemon and shell](#running-mongo-daemon-and-shell)
      - [References:](#references)

<div id='prereq'/>

## Prerequisites:
```console
npm init
npm install --save express body-parser
npm install --save-dev nodemon
npm install --save express-graphql graphql
npm install --save mongoose
// launch

node app.js

// once script entry added to package.json

npm start

browse 
```

<div id='examples'/>

## Examples:

Browse http://localhost:3000/graphql

Under GraphiQL 
```console
mutation {
  createEvent(eventInput: {title:"Test", description: "This is a test", price: 9.99, date: "2019-09-17T19:31:02.531Z"}) {
    title
  }
}
```

Download/Installing/Running MongoDB manually
#### Download MongoDB from website

```console
cd Downloads
mv mongodb-osx-x86_64-3.0.7.tgz ~/
```

#### Extract MongoDB
```console
cd ~/ > tar -zxvf mongodb-osx-x86_64-3.0.7.tgz > mv mongodb-osx-x86_64-3.0.7 mongodb
```

#### Setup directory/permissions where MongoDB will store files
```console
sudo mkdir -p /data/db
sudo chown -R `id -un` /data/db
```

#### Running Mongo daemon and shell
```console
~/mongodb/bin/mongod
~/mongodb/bin/mongo
```

To exit shell ```quit()```
To stop daemon ```ctrl-c```
<div id='references'/>

#### References:
https://www.youtube.com/watch?v=yvEEeKMuxn0
