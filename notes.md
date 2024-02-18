in mongo db dont give allw access from anywhere in netwrok accesss of security section instead use current ip addresss


two approaches of database connection -- a) all codes in index file and executed here when code is load 
b) db file create and write code in connection and import it in index file then execute it.

database connection is mongo through and app connection is through epress.


How does mongoose connect to databases 


in databases two imp words --
1) try catch or promise should be used because problems occurs.
2) database is in another continent so it will take time so async await should be used.


Procedure-
Ist method
1. In this approach is index.js approach in this try catch part in try part connect mongoose will give connect and to connect we need string take variable process env and what is the name of variable of mongodb database link in variable in .env file and add database name also to it which is saved in another folder. to connect this before await should be used.

2.app initialisation also done here for that import expresss and acreate app variable from express and in next to connect part use app express method using listner method 'on' event and callback is made and consolel log and error method.

3. app.listen is used after that and callback port is used and variable process.env is used.


IInd method--
In this create db folder and file and import it into index file
import mongoose and import db name  and create a fuction or variable connectDB and take asynac and try catch method and error method insted pf throw error and use process of node.js and process.exit(1).
In try method tak await and connect and variable process and link name in env of database and database name also given and it can be stored in a variable connectionInstance and console log it as mongoDB connected. and take DB host take connctionInstance anc connection and host. In last export this connctDb.
import connectDB and execute it in index.js file of source and after some time it it will return promise for that use .then and .cathc in this catch if database failed console as callback funcioon and in then use app.listen and process of and port 8000 alternate port and cosole server is running and proces ece port .

what is role of dotenv.
It says as much as possible import and configure this dot env in your application but if we take its method require first in code and after import it will spoil the consistancy of code.
To solve this import dotencv and config it path './env'
it is not used in anywhere like import and require for that it is used as experimental module in package json
In this mongoose and dbName is not imorted because it is already used in connectDb of anther file.

Express uses --
In this req and res and two options are there what req data coming and res data sending for . req.json req.param - any data from url come in params similarly body, qury etca re there and also from cookies also .
In this two middlewares are imporatna cookies-parser and cors .
If you are using middleware app.use is used like app.get
Install both these packages 
now imort both in app.js . already app variableis tkaen from express
now app.use in this cors is taken options are taken like origin proces.env and cross origin and another option credentials as true other options will be available. 
other forms of data are sent like json form etc and for that app.use middlware  is used to limit the data like json limit:16kb. In url also fdifferen types of data is come for this urlencoded is used . and limit also be used.
One more cnfigauration and like static for image, files, folder accesss for public for this app.use middlelware and expres.static is used.


cookieparser - taking cookies from user and set those cookies in format secure cookeis where server uses.
fot this also take app.use middleware and inside pass cookieparser.

Middleware--
It is middle checker before response is sending anything if logged in or not check if user is admin. check if user is logged in. It will check any request is made to database ot any response is sending also it will checks.
Like req, res two more elemens are  there err, next .

In database async is used and try and catch is used for each and every time for this utility file is created and pass function through this and it will send the data when needed and apply wrapper.
For this asynhandler file is created and it wil create method but this function has two call back to avoid try and catch
 const method => () => () . pass method in first callback and in secon pass req res  next  and in wrapper pass promise method an resolve and pas method of and catch err. In this Promise.resolve is invoked.

How to write a standardised of res and req models  


