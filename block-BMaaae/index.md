writeCode

Write code to:-

- create a database named `sports`.

use sports

- list all databases present in local mongod server.

show dbs

- create 3 collections named `cricket`, `football`, `TT` in sports databse.

db.createCollections('cricket')
db.createCollections('football')
db.createCollections('TT')

- add multiple players in those collections which should have fields like `name`, `age` and `email` and `bid_price`.
db.cricket.insertMany({'name':Aaron,'age':24,'email':xxxx@gmail.com,'bid_price':20000},{'name':Baron,'age':24,'email':xxxx@gmail.com,'bid_price':80200},{'name':Caron,'age':24,'email':xxxx@gmail.com,'bid_price':20000})

db.football.insertMany({'name':Aaron,'age':24,'email':xxxx@gmail.com,'bid_price':20000},{'name':Baron,'age':24,'email':xxxx@gmail.com,'bid_price':80200},{'name':Caron,'age':24,'email':xxxx@gmail.com,'bid_price':20000})

- list all collections in sports database.

show collections 

- rename `TT` collection to `tennis`.
db.TT.renameCollection("tennis")

- create a capped collection called `khokho` which should have max 3 documents.
db.createCollections('Khokho',{capped:true,size:100000});

  Try inserting more than 3 and see what happens?
- check whether a collection is capped or not?

db.khokho.isCapped()

- drop all documents from `football` collection.
dbs.football.drop()

- delete cricket collection completely.
dbs.football.remove({})

- delete sports database.
db.dropDatabase();

- check which database you are connected to ?
db

- connect to test database
use testDatabase
