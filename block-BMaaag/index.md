writeCode

Write code to:-

- create a database named `mountains`
 use mountains
- a collection inside that database named `himalayas`

- insert 1 document into that collection `{name: 'Dhauldhar range', height: '4000 mtrs'}`
db.himalayas.update({name: 'Dhauldhar range', height: '4000 mtrs'})

- insert multiple document using insertMany command
db.himalayas.insertMany([{name: 'Dhauldhar range', height: '4000 mtrs'}]})
- find all documents from mountains 
- find a single document using name
