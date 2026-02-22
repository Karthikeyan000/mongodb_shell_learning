# mongodb_shell_learning

A small collection of MongoDB shell exercises and examples used for learning common CRUD, query, and aggregation patterns.

Files
- excercise.mongodb — MongoDB shell commands and examples (insert, find, update, delete, sort, projection, counts, and array queries).
- conn_nodejs/ — Minimal Node.js example for connecting to MongoDB (see `app.js` and `atlas_uri.js`).

Prerequisites
- MongoDB shell (mongo) or mongosh installed and available on your PATH.
- Node.js (for the `conn_nodejs` example).

Quick start
1. To run the shell exercises in `excercise.mongodb` with mongosh:

	mongosh --file excercise.mongodb

	Alternatively, with the classic shell:

	mongo < excercise.mongodb

2. To run the Node.js example:

	cd conn_nodejs
	npm install
	node app.js

What you'll find in excercise.mongodb
- Insert examples: `insertOne()` and `insertMany()` with documents containing nested arrays/objects.
- Query examples: basic `find()` queries, `$in`, `$gt`, `$lt`, `$lte`, `$gte` comparisons.
- Array queries: `$elemMatch` usage to match elements inside arrays (skills, projects, previousCompanies).
- Logical operators: `$and`, `$or` examples and combining operators.
- Update examples: `updateOne()` with `$set`, `updateMany()`, `replaceOne()`, `upsert` option, and `findAndModify()`.
- Delete examples: `deleteOne()` and `deleteMany()` examples.
- Sorting and collation examples demonstrating `.sort()` and `.collation()`.
- Projection examples showing field inclusion/exclusion in `find()` results.
- Counting documents with `countDocuments()`.

Purpose and usage notes
- The file `excercise.mongodb` contains runnable shell snippets you can execute directly against a local MongoDB instance or onto a connected Atlas cluster (update connection details when necessary).
- The examples are written to be educational rather than production-ready; expect to adapt identifiers (like ObjectId values) when running them.

Questions or next steps
- Want me to run the Node example, add a small script to load the exercises automatically, or commit these changes? Say which and I can proceed.
