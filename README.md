# NoSQL Research Lab

## Explainer
Up until now in the cohort we have stored data only in what are known as relational databases (SQL is the most well known type of relational DB querying language). Relational databases structure our data into tables. Today we will learn about a different type of database: a non-relational one. 

## Lab

In this lab you will be researching, either individually or in groups, answer to the following questions about noSQL databases. The intention is for you to spend some time learning about the fundamental differences between the type of databases we have seen before and the new type we will be learning about today. Even more importantly, you will learn about why two types of databases are used, and what situations fit each type of db. 

## Setup

Fork and clone this repository and answer questions as you research directly in the README. You do not have to submit this lab, but you will want to have it on hand for reference in the future. 

# Questions:
1. What does the term noSQL refer to, and what other term is often used synonymously with noSQL?
    * Another term often used to describe noSQL databases is non-relational, to explain how the database is organized into documents/pages, versus tables. 
2. What are some of the common arguments for using a non-relational versus a relational db?
    * Because not all data points in a table are ever used, documents bring down (in theory) storage costs and volume. 
    * Documents are easier and faster to query than tables, and the specificity of querying allows for cheaper costs application maintainers. 
    * Some developers just prefer the document/Mongo modality and find it preferable for managing data, and like using the Mongo tools. 
3. In this class we will be using the document style of non-relational databases. What are the charecteristics of a document based db? 
    * Document based databases store data in individual pages, or documents, over table rows. As an example, a User model would represent a type of document that could be created, and then each individual User would have their own document instance for their account. 
    * Documents are (typically) written in key-value pairs, which can be used for querying. 
4. In this class we will be using Mongo specificially as our no-SQL db. Look into Mongo and answer this question: what is the priamry difference between how Mongo is maintained vrs SQL?
    * MongoDB is developed and maintained by a publicly traded company, MongoDB Inc. As such, the company has specific interests related to how they manage their business, not just concerns around maintaining Mongo itself. 
    * In comparison, SQL is a querying language not owned or managed by one person. A lot of companies make products using SQL, but no one company benefits financially from changes to SQL. The main type of SQL db we used in class, Postgres, is open source. 
5. Mongo DBs are organized into documents. Describe an example of a table in SQL that contains users, and then describe the equivalent DB setup in Mongo.

* **Example user table in Postgres:**

    | id | username   | password | email             |
    |----|------------|----------|-------------------|
    | 1  | annazocher | 12345678 | anna.zocher@ga.co |

* **Example user document in Mongo:**

    ```Mongo
    {   _id: <ObjectID>,
        username: "annazocher",
        password: "12345678",
        email: "anna.zocher@ga.co"
    }
    ```

6. What is an example situation where a Mongo database makes sense versus a non-relational db?
    * MongoDB is a good choice if 1. you, or your company, likes using Mongo over Postgres, and 2. if you want to be able to add data in an unstructured way to a larger database, and not do as much initial organization/stubbing. 



