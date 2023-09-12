# Noknots
[![wakatime](https://wakatime.com/badge/github/lukecp5/noknots.svg)](https://wakatime.com/badge/github/lukecp5/noknots)    

Noknots is a SaaS platform designed to simplify the onboarding process and the maintaining of e-commerce products. It automatically crawls the websites of e-commerce sellers, imports and displays some of their products with the proper classification, allergens, and small description already pre-filled. 

The Noknots backend is a REST API built on an Express.js server that uses [Sequelize](https://sequelize.org/master/) to interact with a MySQL database, which will serve as place to store all customer and product data. Sequelize is a promise-based Node.js ORM(Object Relation Mapping) for Postgres, MySQL, MariaDB, SQLite and Microsoft SQL Server which will be used to help maintaining a clean database access.

This backend has the API routes that point to each of the standard [CRUD] operations for each data group. The routes can be used to:
- Create categories, products, tags
- View categories, products, tags
- Establish associations between the different entities
- Update categories, products, & tags
- Delete entries from the database

This project will gain different features over the next months and an MVP will be created out of it into the branch called 'mvp'.


## **Table of contents**

- [Noknots](#noknots)
  - [Table of contents](#table-of-contents)
  - [Installation](#installation)
  - [Usage](#usage)
  - [Contributing](#contributing)
  - [Demo Video](#demonstration-video)
  - [Built With](#built-with)
  - [License](#license)

## **Installation**

Start with cloning this repo on your local machine:

```sh
$ git clone https://github.com/lukecp5/noknots.git
$ cd noknots
```

To install and set up the application, run:
```sh
$ npm install noknots
```

You will also need to place a .env file in the root directory of the project, in order to connect to your MySQL database. Here's an example:

file: .env
```
DB_NAME=library_db
DB_PASSWORD=
DB_USER=root
```


## **Usage**
<sub><sup>This section assumes you have installed the application, and created the .env file in the root directory.</sub></sup>

To finish the set-up the application, complete the following steps:
1. Create a MySQL database on your local machine using the *schema.sql* file located in the /db/ directory(From the MySQL CLI, source db/schema.sql)
2. Seed the database with sample data to be used for testing purposes(Run *npm run seed* from inside the root directory of the project)

Now you're ready to start the application! You can start the server by running: 
```
npm start
```

The server is running, now you can make requests to it through your desired method. If you're new to the backend, I suggest trying out [Postman](postman.com)



## **Built With**
* [**Node.js**](https://nodejs.org/en/about/)
*  - [Sequelize](https://www.npmjs.com/package/sequelize)
*  - [Express.js](https://www.npmjs.com/package/express)
* [**Visual Studio Code**](https://code.visualstudio.com/)



## **Demonstration Video**
If you'd like to see a full demo of the application, please visit the following link: [Demo Video on Google Drive](https://drive.google.com/file/d/1gdSIFayRsXjm4BekD5eJcBi1v77JLgIB/view?usp=sharing)


## **Contributing**

1.  Fork it!
2.  Create your feature branch: `git checkout -b my-new-feature`
3.  Add your changes: `git add .`
4.  Commit your changes: `git commit -am 'Add some feature'`
5.  Push to the branch: `git push origin my-new-feature`
6.  Submit a pull request :sunglasses:


## **Author**
**Josip Grgic**   
LinkedIn: [@josipgrgic](https://www.linkedin.com/in/luke-poirrier)  
Email: [josip.grgic@noknots.com](mailto:josip.grgic@noknots.com)  
Portfolio: [ichundmeinewelt.com](http://ichundmeinewelt.com)  


## **License**
This application is licensed under the MIT License, you can find the full license information [here](http://github.com/lukecp5/noknots/LICENSE.txt)
```