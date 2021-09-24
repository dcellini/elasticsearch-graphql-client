# 🚀 ElasticSearch, GraphQL, React, Node+Express🤯! How ?

Simple application using React+GraphQL, ElasticSearch as full-text search and Node JS
[medium.com/@andrewrymaruk](https://medium.com/@andrewrymaruk/elasticsearch-graphql-react-node-express-how-cb2c2cc708f8)

![Simple application using React+GraphQL, ElasticSearch as full-text search and Node JS](https://miro.medium.com/max/1600/0*CkvXp7vOOVgcGt6A.gif)

# How to get this app working

**To run the docker containers**
Navigate to the 'server' folder and run the following command
`docker-compose -f ./file_elastic_kibana_latest.yml up`

**Add document to elasticsearch or delete documents and index**
If starting for the first time...

In the server folder run...
`node server.es.create.js`
to create an index

If you wish to delete an index
`node server.es.delete.js`

To bulk import records to elasticsearch
`node server.es.bulk.js`

You should be able to access kibana and run elasticsearch queries at
http://localhost:5601/

**Next to get graphql running**
Navigate to server folder and run
`node server.js`
You should be able to access graphql at
http://localhost:9100/graphql

**Now for React**
In the root folder (level above survey), run...
`yarn start`
You can access the front end at
http://localhost:9999
