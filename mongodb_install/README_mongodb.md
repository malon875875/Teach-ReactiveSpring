# Info
* https://www.bmc.com/blogs/mongodb-docker-container/
  
# Install MongoDB
* docker pull mongo 
* docker-compose up -d
* The database is bind-mounted to the volume /Teach-ReactiveSpring/mongodb_install/database

# Interact with MongoDB
* docker exec -it mongodb bash
* in the container, type these commands
    * mongo
      * use food
      * db.createCollection("fruits")
      * db.fruits.insertMany([ {name: "apple", origin: "usa", price: 5}, {name: "orange", origin: "italy", price: 3}, {name: "mango", origin: "malaysia", price: 3} ])
      * db.fruits.find().pretty()
      * exit
    * exit
* data is persisted in /Teach-ReactiveSpring/mongodb_install/database