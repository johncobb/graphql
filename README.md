# Learning GraphQL

## Table of contents
- [Learning GraphQL](#learning-graphql)
    - [Table of contents](#table-of-contents)
    - [Prerequisites:](#prerequisites)
    - [Examples:](#examples)
            - [References:](#references)

<div id='prereq'/>

## Prerequisites:
```console
npm init
npm install --save express body-parser
npm install --save-dev nodemon
npm install --save express-graphql graphql
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
query {
    events
}

mutation {
    createEvent(name: "John C")

}
```

#### References:
https://www.youtube.com/watch?v=yvEEeKMuxn0
