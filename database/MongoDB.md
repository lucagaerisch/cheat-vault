# MongoDB

MongoDB is a document database that stores data in `JSON-LIKE` documents, meaning fields can vary from document to document and data structures can be changed over time.

Official Docs: [MongoDB Docs](https://www.mongodb.com/docs/)

## Installation

MongoDB can be downloaded on their official website:
[MongoDB Compass](https://www.mongodb.com/try/download/compass) | [MongoDB Server](https://www.mongodb.com/try/download/community) | [MongoDB Atlas](https://www.mongodb.com/try) | [MongoDB Shell](https://www.mongodb.com/try/download/shell)

MongoDB Shell can also be installed via Node.js (NPM).

```shell
npm install -g mongosh
```

## Monitoring

To enable monitoring on a standalone database, you need to enable it first with the following command:

```shell
db.enableFreeMonitoring()
```

Here is an example of the monitoring website. This website is directly hosted by MongoDB and can be accessed with a unique link that was created by the upper command.

---

#database #nosql #json 