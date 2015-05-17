title: "Hapi Hapi Swag Swag (with swagger and postgres)"
date: 2015-05-17 01:03:24
tags:
- Node.js
- Swagger
- PostgreSQL
---

Let's check the awesomeness of <a href="http://hapijs.com" target="_blank" rel="external">Hapi</a>. It is a framework for building web apps, services and APIs, it is ultra non-bullshit and we are going to check how to create documented REST (with the almost de-facto ruler <a href="http://swagger.io" target="_blank" rel="external">Swagger</a>) and connect to <a href="http://www.postgresql.org" target="_blank" rel="external">PostgreSQL</a>.

First we create a sample table in Postgres:

```
CREATE TABLE example_table
(
  idexample_table bigserial NOT NULL,
  data character varying(100),
  CONSTRAINT pk_idexample_table PRIMARY KEY (idexample_table)
);
```

Then we initiate a node project and install hapi, this will assume we'll use <strong>index.js</strong> as main file and generate a <strong>package.json</strong> file:

```
mkdir hapi-swagger-postgres
cd hapi-swagger-postgres
init npm
npm install --save hapi
```

(Note that we also studied the <a href="http://hapijs.com/tutorials" target="_blank" rel="external">Hapi tutorials</a> and recommend you do so too)

Create a file named <strong>index.js</strong>

.... Continuará!