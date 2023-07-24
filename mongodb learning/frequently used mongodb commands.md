1. **db**: This command allows you to switch to a specific database. For example, `use mydatabase` will switch to the "mydatabase" database.
    
2. **show databases**: This command lists all the databases in your MongoDB server.
    
3. **show collections**: This command displays all the collections in the current database.
    
4. **db.collectionName.find()**: This command retrieves all documents from a collection. For example, `db.users.find()` will return all documents in the "users" collection.
    
5. **db.collectionName.findOne()**: This command retrieves a single document from a collection. For example, `db.users.findOne()` will return the first document in the "users" collection.
    
6. **db.collectionName.insertOne(document)**: This command inserts a single document into a collection. For example, `db.users.insertOne({ name: "John", age: 30 })` will insert a document with the name "John" and age 30 into the "users" collection.
    
7. **db.collectionName.insertMany([document1, document2, ...])**: This command inserts multiple documents into a collection. For example, `db.users.insertMany([{ name: "John", age: 30 }, { name: "Jane", age: 25 }])` will insert two documents into the "users" collection.
    
8. **db.collectionName.updateOne(filter, update)**: This command updates a single document that matches the filter criteria in a collection. For example, `db.users.updateOne({ name: "John" }, { $set: { age: 35 } })` will update the age of the document with the name "John" in the "users" collection to 35.
    
9. **db.collectionName.updateMany(filter, update)**: This command updates multiple documents that match the filter criteria in a collection.
    
10. **db.collectionName.deleteOne(filter)**: This command deletes a single document that matches the filter criteria in a collection.
    
11. **db.collectionName.deleteMany(filter)**: This command deletes multiple documents that match the filter criteria in a collection.
    
12. **db.collectionName.aggregate(pipeline)**: This command performs aggregation operations on a collection using a series of stages specified in the pipeline. Aggregation allows you to perform complex data transformations and analysis.
    
13. **db.collectionName.createIndex(keys, options)**: This command creates an index on specified keys in a collection. Indexing helps improve query performance.
    
14. **db.collectionName.dropIndex(indexName)**: This command drops an index from a collection.