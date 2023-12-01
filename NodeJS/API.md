## REST API
FOLLOW PARTICULAR SET UP RULE and use http protocol TO INTRATCT WITH THE API . <br/>
Axios<br/>
await axios .get(url,config)<br/>
await axios.post(url,body,config) <br/>
rest API is resource based, so it is an API that is centered around resources and uses a unique resource identifier, also known as a resource locator.
## HTTP Requests - HyperText Tranter Protocol
- Helps to transfer data from computer to another.<br/>
- Important terminology<br/>
- GET- getting resource (html,text,data)yarn workspace mouana-diy-platform develop --watch-admin<br/>
- POST-Sending resource ( example  sign in data)<br/>
- Update    1) PUT- Replace resource<br/>
            2) PATCH-Patch up resource <br/>
            3) DELETE- delete resource <br/>
- req.rawHeaders- are key pair value pairs that come from where the request is originated .<br/>
- HTTP Response Status code -https://developer.mozilla.org/en-US/docs/Web/HTTP/Status<br/>
## REST APIs
These are the most popular and flexible APIs found on the web today. The client sends requests to the server as data. <br/>
The server uses this client input to start internal functions and returns output data back to the client.<br/>
## Formatting API REQUESTS.**
**Private API**- don’t document for other to use. Severs only your  own front end and not somebody else. <br/>
**Public API**- document for other to use. Anyone can use to interact.<br/>
## API endpoints** <
**basic structure** - Base URL/Endpoint Endpoint can be different for different purpose.<br/>
## Query Parameters**<br/>
start with ?,follwoed by key and value pair.<br/>
base Url/Endpoint/?query=value<br/>
&- to add more parameters<br/>
base Url/Endpoint/?query=value&&query2=value<br/>
Path parameters<br/>
they change and are usually to fins some specific resource that exits.<br/>
Base URL/Endpoint/{path-parameters} 
# API Authencation**
1) No Authencation 
2) Basic - conervt to Basic 64 encoding
3) API Key
