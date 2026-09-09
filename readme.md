localhost
127.0.0.1-Ip address
every request from client has a pair of {request,response}
ctrl+c-for stopping the server.
npm-node package manager
used to install,run,uninstall any program and package
-npm install <packagename>
-npm uninstall <packagename>
to use npm,the project must be npm project,
to create npm project we can use
-npm init -y
-it creates a package.json file automaticallly
package.json holds all the information related to install packages from npm
-it also creates a folder node_modules automatically
-node_modules holds the package/library files
-generally we ignore the node_modules by .gitgnore
nodemon-it restart the server automatically when file changes
npm i nodemon -D
note: -D flag will install this
package as developer dependency
-to execute any program,update the package.json file then start the server 
start-it will execute the app on deployment
dev-it will start server in devlopment phase (only for developer)
res: it will return contents (json/html/plain) to the user/client 
req:it will retrive the information from client to the server
server send also statuscodes to the client,that indicates the error/success message
# status codes 
-200-ok
-201-created
400-unauthorized
403-forbidden
404-not found
500-internal server error
##content type
text/plain
text/html
application/json
text/css
the content type and status code can be send back to client by two ways
1.res.writehead
2.res.setheader
3.res.statusCode
##response as html content
1. res.end
end("any html content/tag")
2. html file
read by createreadstream
pipe with res
2. html content
send any html tags/content by using
res.end('<any html tag>')
json-javascript object notation
servers return data only not html contents because html contents will be written by frontend developer the data is in json format.
json always stores data in key ,valuer pair enclosed by {} array can be stored by square [] one pair of {} bracket will represent one object and its property will be separated by , ex-
## JSON
```
 {
    id:1,
    name:'mobile',2
    price:2500,
    rating:4.5
    review:200

 }
```
