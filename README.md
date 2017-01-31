Example:
$ cd ~

$ mkdir html

$ cd html

$ docker run -d -p 8080:80 -p 8081:443 -v $(pwd)/test:/var/www/html --name apache angeloevaldez/centos7-http

$ echo "Hello World" > test/index.html

$ curl localhost:8080
Hello World

