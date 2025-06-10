MongoDB Fundamentals Assignment – My Setup Instructions

How to Run My Scripts

Install Dependencies:
Run this command in the terminal to install the MongoDB Node.js driver:
npm install mongodb

Insert Sample Book Data:
To populate the database, run:
node insert_books.js

MongoDB Setup:
I used MongoDB Compass to view data.
Database name: plp_bookstore
Collection name: books

MongoDB Shell (mongosh):
I ran my queries using mongosh by typing:
mongosh
Then switched to the database using:
use plp_bookstore

Query File:
All my MongoDB queries are in queries.js


Aggregation Pipeline Example:
db.books.aggregate([
{ $group: { _id: "$genre", averagePrice: { $avg: "$price" } } }
])

Tools Used

VS Code
Node.js v18+
MongoDB Shell
MongoDB Compass

Screenshots are in the Images file