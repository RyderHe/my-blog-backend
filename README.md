# Node.js 

## Init

`npm init -y`

## Install

:white_check_mark: ` npm i -s express`

:white_check_mark: `npm i -s body-parser` -> allow server to extract JSON data sent along request

:white_check_mark: `npm install --save-dev @babel/core @babel/node @babel/preset-
env`  -> allows Node.js to use ES6

* `.babelrc`: 

```
{
    "presets": ["@babel/preset-env"]
}
```

* `npx babel-node src/server.js`: run the server

:white_check_mark: `npm install --save-dev nodemon` -> automatically restart server when a change happens

* run `npx nodemon --exec npx babel-node src/server.js` instaead of the above
* Or, change `package.json` and run `npm start`

```
  "scripts": {
    "start": "npx nodemon --exec npx babel-node src/server.js"
  },
```

:white_check_mark: :triangular_flag_on_post: `npm install --save mongodb` -> allow modify mongodb inside express server

# MongoDB

:white_check_mark: `mongod` -> start mongoDB & leave it running

:white_check_mark: `mongo` -> open mongo shell

:white_check_mark: `Ctrl + C` -> exit mongo shell

## Some Basic Commands

:small_blue_diamond: create & switch to new database: `use my-db`

:small_blue_diamond: create collection and insert data : `db.my-collection.insert([{name: 'record1', type: 'comics'}, {name: 'record2', type: 'comics'}])`

:small_blue_diamond: show all data in the collection: `db.my-collection.find()`

* `db.my-collection.find().pretty()`

* `db.my-collection.find({name: 'record1}).pretty()`

* `db.my-collection.findOne({name: 'record1})` [cannot use pretty with findOne]


