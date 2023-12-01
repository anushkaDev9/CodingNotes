## express  basic code
  <pre>
  import express from ‘express
  const app=express()
 appp.listen(3000,()⇒{ console.log(”server running on port 3000.”);)};
-3000-port (location of the server listening the response from user)
console.log(”server running on port -callback
  </pre>
## Install express
- *npm install express*
- start server- node filname.js
- nodemon- automatical;y restarts the node application.
- If you want the server to automatically restart whenever you make changes, you can use Nodemon by installing it globally (`npm install -g nodemon`) and then running `nodemon filename.js`.
- ### localhost
- when we don’t have server on internet and we want to host server locally
- http://localhost:7000
- netstat -ano | findstr “LISTENING” - check which port is working in yout terminal (WINDOW)
### direname - directory name 
fileURLToPath- 
### MiddleWare
- they work with request
- BodyParser - request bodies before your handlers.
 used manly for forms (pres porcessing middlewaree)
Morgan- looger middler 
Custom Middleware -
