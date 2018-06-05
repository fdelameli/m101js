Use mongorestore to restore the dump into your running mongod. Do this by opening a terminal window (mac) or cmd window (windows) and navigating to the directory so that the dump directory is directly beneath you. Now type:

```
mongorestore dump
```

Note you will need to have your path setup correctly to find mongorestore.

Then install all the dependencies listed in the 'package.json' file. Calling 'npm install' with no specific package tells npm to look for 'package.json':

```
npm install
```

This should create a "node_modules" directory with all the dependencies. Now run the application to get the answer to hw1-3:

```
node app.js
```

If you have all the dependencies installed correctly, this will print the message 'Express server listening on port 3000'. Navigate to 'localhost:3000' in a browser and enter the text that is displayed on that page in the text box below.
