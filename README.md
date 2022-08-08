https://www.youtube.com/watch?v=iCZcE-JKbyY&list=PLwJWw4Pbl4w_oHjPIjkdVtwLeQECK08jv&index=2

npm install

# Paramètres de configuration .env

npm run dev

Database connection OK
This server is running on port 8888. Have fun !

# JWT server.js
app.use('/users', checkTokenMiddleware, user_router)
// app.use('/users', user_router)

# Tester avec Postman
PUT localhost:8888/users

Body x-www-form-urlencoded

nom : croquet
prenom : patrick
pseudo : pat@
email : patrick.croquet@afpa.fr
password : patrick@94010

# JWT 
jwt.io

const jwt = require('jsonwebtoken')

www.npmjs.com/package/jsonwebtoken

# Tester avec Postman
POST localhost:8888/auth/login

Body x-www-form-urlencoded

email : patrick.croquet@afpa.fr
password : patrick@94010

{
    "access_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6MSwibm9tIjoiY3JvcXVldCIsInByZW5vbSI6InBhdHJpY2siLCJlbWFpbCI6InBhdHJpY2suY3JvcXVldEBhZnBhLmZyIiwiaWF0IjoxNjU4OTEzOTUxLCJleHAiOjE2NTg5MTc1NTF9.eJxupIkzXgOFPX5ShmRQDBcC6DUg2vJhJZye5hcooyM"
}

J'envoie l'access_token dans jwt.io

PAYLOAD:DATA
{
  "id": 1,
  "nom": "croquet",
  "prenom": "patrick",
  "email": "patrick.croquet@afpa.fr",
  "iat": 1658913951,
  "exp": 1658917551
}