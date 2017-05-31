# nodejs 

docker build -t angeloevaldez/nodejs . 

docker run -dit -p 8000:8000 --name nodejs angeloevaldez/nodejs 

docker run -dit -p 8000:8000 --name nodejs angeloevaldez/nodejs example/hello.js

docker run -dit -p 8000:8000 -v $(pwd)/example:example/ --name nodejs angeloevaldez/nodejs 
