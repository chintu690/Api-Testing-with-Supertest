# Api-Testing-with-Supertest

//SetUp

1. Create a node project in Your Local

2. install Jest, jest-stare for generating custom test
    npm install jest jest-stare jest-serial-runner --save-dev  
    
    npm run test command will invoke the test parameter with the following:

NODE_TLS_REJECT_UNAUTHORIZED=0: ignores the SSL certificate
jest: runs the framework with the configurations defined under Jest block
--reporters: default jest-stare 
--coverage: invokes test coverage
--detectOpenHandles: for debugging
--runInBand: serial execution of Jest tests
--forceExit: to shut down cleanly
--testTimeout = 60000 (custom timeout, default is 5000 milliseconds)
    
3. add tests scripts to your package.json file.
   "scripts": {
  "test": "jest",
  "test:watch": "jest --watch"
   }
Jest configurations:

4. Install Supertest for endpoint testing 
   npm install supertest --save-dev
   


5. Testing endpoints with SuperTest

SuperTest is a node library, superagent driven, to extensively test Restful web services. It hits the HTTP server to send requests (GET, POST, PATCH, PUT, DELETE ) and fetch responses

Install Supertest for endpoint testing 
   npm install supertest --save-dev
   
   "devDependencies": {
    "jest": "^26.1.0",
    "jest-serial-runner": "^1.1.0",
    "jest-stare": "^2.0.1",
    "supertest": "^4.0.2"
  }
  
  After All the required dependencies are installed and our package.json looks like:
  
  {
  "name": "apitestingjest",
  "version": "1.0.0",
  "description": "APi Testing with Jest and SuperTest",
  "main": "index.js",
  "scripts": {
    "test": "NODE_TLS_REJECT_UNAUTHORIZED=0 jest --reporters default jest-stare --coverage --detectOpenHandles --runInBand --testTimeout=60000",
    "test:watch": "jest --verbose --watchAll"
  },
  "author": "",
  "license": "ISC",
  "devDependencies": {
    "jest": "^26.1.0",
    "jest-serial-runner": "^1.1.0",
    "jest-stare": "^2.0.1",
    "supertest": "^4.0.2"
  }
}

6.npm run test command will invoke the test parameter with the following:

NODE_TLS_REJECT_UNAUTHORIZED=0: ignores the SSL certificate
jest: runs the framework with the configurations defined under Jest block
--reporters: default jest-stare 
--coverage: invokes test coverage
--detectOpenHandles: for debugging
--runInBand: serial execution of Jest tests
--forceExit: to shut down cleanly
--testTimeout = 60000 (custom timeout, default is 5000 milliseconds)
  
