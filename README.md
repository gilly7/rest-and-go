# rest-and-go
A basic online store API written to learn Go Programming Language

This API is a pretty basic implementation of an online(e-commerce) store.
- You can perform basic CRUD(CREATE, READ, UPDATE and DELETE) operations
- SEARCH on a predefined database of products 
- Only Authenticated users can Add, Update and Delete products from database
- Authentication is based on JWT(JSON web Tokens) Tokens
- API is backed by a predefined Mongo DB database hosted on [mLab](https://mLab.com)
- This API also lives on [Heroku](https://www.heroku.com) - https://gruesome-monster-22811.herokuapp.com/ 

See [API Documentation and Usage](#api-documentation-and-usage) below on how to use it.

## Directory Structure
```
rest-and-go/
    |- Godeps/             - Contains info about all dependencies of the project
    |- store/              - Contains main API logic files 
        |- controller.go  - Defines methods handling calls at various endpoints
        |- model.go       - User and Product models
        |- repository.go  - Methods interacting with the database
        |- router.go      - Defines routes and endpoints
    |- vendor/             - Dependency packages, necessary for deployment
    |- .gitignore
    |- LICENSE
    |- Procfile             - Procfile for herkou deployment
    |- README.md
    |- dummyData.js         - Script to populate local mongodb with dummy data
    |- main.go              - Entry point of the API
  
```


## Setup

### Golang Development Setup

Inspired by [this article](https://medium.com/@gautamprajapati/writing-a-simple-e-commerce-website-api-in-go-programming-language-9f671324b4dd)
