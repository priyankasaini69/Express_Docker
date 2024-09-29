## Testing express application by deploying mongo database in docker
This app shows a simple express application
- get request for viewing the products
- post request for adding a new product
- mongodb for data storage 

All components are docker-based
### With Docker Compose

#### To start the application

Step 1: Build the application 
    docker build .
The dot "." at the end of the command denotes location of the Dockerfile.

Step 2: start mongodb

    docker-compose -f docker-compose.yaml up

Step 3: go to postman for ease
    a) GET - http://localhost:4000/products
    b) POST - http://localhost:4000/products

#### To build a docker image from the application

    docker build -t express-app:1.0 .  
    
The dot "." at the end of the command denotes location of the Dockerfile.