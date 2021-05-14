writeCode

Write command to

- List collections from a database.
show collections
- create a new collection in your country database which you created recently.
use Country
db.createCollection('India')

Write code to:-

- crate a database named `weather`
use weather
- create a capped collection named `temperature` with maximum of 3 documents and try inserting more than 3 to see the result.
db.createCollection('temperature',{capped:true,size:100000})
- create a simple collection named `humidity`
db.createCollection('humidity')
- check whether `temperature` collection is capped or not ?
- Delete `humidity` collection and then the entire database(weather).
db.humidity.remove({})
