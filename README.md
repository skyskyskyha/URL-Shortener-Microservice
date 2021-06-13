# API Project: URL Shortener Microservice for freeCodeCamp
这个project用到了MongoDB数据库，用于给每个网站一个编号，并能实现跳转到对应编号的网站
参考一下几个攻略：
https://baristure.medium.com/freecodecamp-apis-and-microservices-url-shortener-microservice-720951cb68db
源代码：
https://github.com/baristure/FreeCodeCampProjects
视频：
https://www.youtube.com/watch?v=dvCIN_pav8o

### User Stories

1. I can POST a URL to `[project_url]/api/shorturl/new` and I will receive a shortened URL in the JSON response. Example : `{"original_url":"www.google.com","short_url":1}`
2. If I pass an invalid URL that doesn't follow the valid `http(s)://www.example.com(/more/routes)` format, the JSON response will contain an error like `{"error":"invalid URL"}`. *HINT*: to be sure that the submitted url points to a valid site you can use the function `dns.lookup(host, cb)` from the `dns` core module.
3. When I visit the shortened URL, it will redirect me to my original link.


#### Creation Example:

POST [project_url]/api/shorturl/new - body (urlencoded) :  url=https://www.google.com

#### Usage:

[this_project_url]/api/shorturl/3

#### Will redirect to:

https://www.freecodecamp.org/forum/
