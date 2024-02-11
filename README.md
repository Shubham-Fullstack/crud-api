# crud-api
x-x--x-x-x-x-x-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
"cors": "^2.8.5",
    "json-serve": "^0.1.0",
    "json-server": "^0.17.1"

 x---------x--x-x--x-x-x-x--x-x-x

 const jsonServer = require("json-server"); // importing json-server library
const server = jsonServer.create();
const router = jsonServer.router("db.json");
const middlewares = jsonServer.defaults();
const port = process.env.PORT || 8080; //  chose port from here like 8080, 3001

server.use(middlewares);
server.use(router);

server.listen(port);
