`npm init -y`

` npm i -s express`

`npm i -s body-parser` -> allow server to extract JSON data sent along request

`npm install --save-dev @babel/core @babel/node @babel/preset-
env`  -> allows Node.js to use ES6

* `.babelrc`: 

```
{
    "presets": ["@babel/preset-env"]
}
```

* `npx babel-node src/server.js`: run the server

`npm install --save-dev nodemon` -> automatically restart server when a change happens

* run `npx nodemon --exec npx babel-node src/server.js` instaead of the above
* Or, change `package.json` and run `npm start`

```
  "scripts": {
    "start": "npx nodemon --exec npx babel-node src/server.js"
  },
```