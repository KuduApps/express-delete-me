To create the express app:

From inside an existing web role directory
(1) npm install express
(2) express  (respond 'y' to overwrite)
(3) del server.js
(4) mv app.js server.js
(5) npm install
9^) in server.js, change the listen port:

- app.listen(3000);

becomes 

- app.listen(process.env.port);


Note that the certificate in the TestApps directory can be used as an SSL certificate for these apps