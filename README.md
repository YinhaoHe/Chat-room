# Chat-room
## Getting Started
These instructions will get you a copy of the project up and running on your local machine for development purposes.

### Running the Application
1. Install Node.js
2. Download/clone this repository
3. Open the ```Chat-room``` folder
    - Go to the ```client``` folder and type ```yarn install``` to gather all the necessary packages 
    - Go to the ```server``` folder and type ```npm install``` to gather all the necessary packages
4. Follow this [tutorial](https://fullstackopen.com/en/part3/saving_data_to_mongo_db) to set up your MongoDB database
  
    - When you are done, create a file named ```config.js``` and put it under the ```server/util``` directory
5. Follow the template below for your ```config.js``` file
    - Should be simple with the SRV address provided by Atlas
    ``````
    const URI = 'mongodb+srv://<USERNAME>:<PASSWORD>@<SERVER-ADDRESS>/<APP-NAME>?retryWrites=true';
    module.exports = { URI }; 
    ``````
6. Type ```yarn start``` to run the front-end code and ```npm start``` for the back-end code
  
    - The front-end should be running on ```localhost:3000 ```and ```localhost:3001``` for the back-end unless you have other applications running simultaneously
7. Hit ```Ctrl+C``` on terminals running the front-end and back-end code to stop running

## Built With
### Front-end
- React.js
  - Material-UI
- UUID
- Socket.IO
### Back-end
- Node.js
  - nodemon
- Express.js
  - CORS
- MongoDB Atlas
  - Mongoose
- Socket.IO
