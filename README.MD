# THIS IS EXPRESS TEST SERVER

server.js

const express = require('express');
const app = express();
const PORT = process.env.PORT || 3000;

app.listen(PORT, () => {
	console.log(`Server listening on ${PORT}`);
});

app.get('/', (req, res) => {
	res.status(200).send('Hello world!');
});
