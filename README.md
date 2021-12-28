# Express-Github-API
This a REST microservice developed using Expressjs. 

# Functional specs
* The API lists the languages used by the trending public Github repos.
* It calculates the total number of the repos (100 repos - repos with `null` language) 
* For every language, it returns : 
  * The number of repos using that language.
  * The list of those repos.
# Technologies Used
* [Nodejs](https://github.com/nodejs/node) : JavaScript runtime enviromment.
* [Express](https://github.com/expressjs/express):  Node.js web application server framework.
* [axios](https://github.com/axios/axios) : Promise based HTTP client for the browser and Node.js.
* [Moment.js](https://github.com/moment/moment) : JavaScript date library.

# Available Endpoints
Verb | endpoint | description |
--- | --- | --- |
GET | api/repos/ | Lists the trending languages in the last 30 days |
GET | api/repos/{date} | Lists the trending languages in the last 30 days from the given date|

# Expected response

```json
{
  "total_count": "x",
  "result": [
     {
         "language": "languageX",
         "number of repos": "x",
         "repos ": [
             "repo1",
                 ...
             "repoN"
         ]
     },
        ...
  ]
}
```

# Getting Started

 * Clone the repo :
 
```shell
 git clone https://github.com/Selharem/Express-Github-API.git
```
 * Install the dependencies : 
 
```shell
 npm install
```
* Start the server : 
```shell
 npm start
```

<p align="center">Made with ❤️ By <a href="https://github.com/Selharem">Elharem Soufiane</a></>