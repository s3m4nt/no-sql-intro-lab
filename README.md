# NoSQL Research Lab

## Explainer
Up until now in the cohort we have stored data only in what are known as relational databases (SQL is the most well known type of relational DB querying language). Relational databases structure our data into tables. Today we will learn about a different type of database: a non-relational one. 

## Lab

In this lab you will be researching, either individually or in groups, answer to the following questions about noSQL databases. The intention is for you to spend some time learning about the fundamental differences between the type of databases we have seen before and the new type we will be learning about today. Even more importantly, you will learn about why two types of databases are used, and what situations fit each type of db. 

## Setup

Fork and clone this repository and answer questions as you research directly in the README. You do not have to submit this lab, but you will want to have it on hand for reference in the future. 

# Questions:
1. What does the term noSQL refer to, and what other term is often used synonymously with noSQL?
    noSQL databases are also known as non-relational databases. Non-relational databases are document oriented. Like file folders that hold information. 

2. What are some of the common arguments for using a non-relational versus a relational db?
    * Simplicity
    * Data Accuracy
    * Easy access to data
    * Data integrity
    * Flexible - can create new relations between tables without sacrificing integrity
    * Open source

    Non-relational databases are often used when large quantities of data need to be organized. For example, a large store might have a database in which each customer has their own document containing all of their information, from name and address to order history and credit card information.

3. In this class we will be using the document style of non-relational databases. What are the charecteristics of a document based db? 
    * flexible schema
    * Universal: JSON Files!
    * Powerful: Query data any way that you need
    * Distributed: Resilient and globally scalable

4. In this class we will be using Mongo specificially as our no-SQL db. Look into Mongo and answer this question: what is the primary difference between how Mongo is maintained vrs SQL?
    The way they handle data. In SQL databases, data is stored in form of traditional 2 dimensional row-column structure while in MongoDB rich data document model is followed, which allows storage of any type of data.

5. Mongo DBs are organized into documents. Describe an example of a table in SQL that contains users, and then describe the equivalent DB setup in Mongo. 
    The equivalent Mongo setup would contain a structure with keys and objects.

6. What is an example situation where a Mongo database makes sense versus a non-relational db?
    For example, a large store might have a database in which each customer has their own document containing all of their information, from name and address to order history and credit card information.    
