# nodejs 

example:

$ docker build -t angeloevaldez/nodejs git@github.com:angelovaldez/nodejs.git 

$ docker run -dit -p 8000:8000 --name nodejs --rm angeloevaldez/nodejs 

$ docker run -dit -p 8000:8000 --name nodejs --rm angeloevaldez/nodejs example/hello.js

$ mkdir example
$ docker run -dit -p 8000:8000 -v $(pwd)/example:/home/example --name nodejs --rm angeloevaldez/nodejs

$ docker run -dit -p 8000:8000 -v (pwd)/example:/home/example --name nodejs --rm angeloevaldez/nodejs example/app.js 

Test:
$ curl -i http://localhost:8000 

HTTP/1.1 200 OK
Content-Type: text/plain
Date: Wed, 31 May 2017 18:15:33 GMT
Connection: keep-alive
Transfer-Encoding: chunked

Hello World
