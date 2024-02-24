#init npm
Run npm init
Run npm i express pg sequelize

#Start app docker compose
Run docker compose build
Run docker compose up -d

#test connection db
psql -h localhost -p 5432 -U postgres -W -d testdb

#test connection crud
GET http://localhost:3000/users

#test create crud
POST http://localhost:3000/users

BODY 
{
    "title": "Node Tut #3",
    "description": "Tut#3 Description"
}
