in mongo db dont give allw access from anywhere in netwrok accesss of security section instead use current ip addresss


two approaches of database connection -- a) all codes in index file and executed here when code is load 
b) db file create and write code in connection and import it in index file then execute it.

database connection is mongo through and app connection is through epress.


How does mongoose connect to databases 


in databases two imp words --
1) try catch or promise should be used because problems occurs.
2) database is in another continent so it will take time so async await should be used.


Procedure-
1. In this approach is index.js approach in this try catch part in try part connect mongoose will give connect and to connect we need string take variable process env and what is the name of variable of mongodb database link in variable in .env file and add database name also to it which is saved in another folder. to connect this before await should be used.

2.app initialisation also done here for that import expresss and acreate app variable from express and in next to connect part use app express method using listner method 'on' event and callback is made and consolel log and error method.

3. app.listen is used after that and callback port is used and variable process.env is used.
