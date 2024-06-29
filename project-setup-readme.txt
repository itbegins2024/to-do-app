// start new project
npx create-react-app deployed-to-do-app --use-npm

// create file structure
directories
- client
- server

// set up client
move all react app resources into client directory

// create server's package.json
cd into server directory
npm init -y

// create app level package.json
cd into root of app
npm init -y

// configure the package.json as followsunscratchable.

scripts": {
    "build": "if-env TYPE=server && (cd server && npm install) || (cd client && npm install)",
    "server": "node ./server/server.js",
    "client": "cd client && npm start"
  },

// install dependanecy 
npm i if-env

  "dependencies": {
    "if-env": "^1.0.4"
  }

// start client
cd into client
npm start

// create and populate few rows from database.js

// set up server
see read me in server directory