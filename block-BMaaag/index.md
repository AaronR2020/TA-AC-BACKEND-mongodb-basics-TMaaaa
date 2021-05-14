writeCode

Write code to:-

- create a database named `mountains`
use mountains

- a collection inside that database named `himalayas`
use himalayas
db.createCollection('mountains');

- insert 1 document into that collection `{name: 'Dhauldhar range', height: '4000 mtrs'}`
db.mountains.insert({name: 'Dhauldhar range', height: '4000 mtrs'});

- insert multiple document using insertMany command
db.mountains.insertMany([{name: 'Dhauldhar range', height: '4000 mtrs'},{name: 'Sorm range', height: '1000 mtrs'}])

- find all documents from mountains
db.mountains.find();

- find a single document using name
db.mountains.find({name:'Dhauldhar range'});
