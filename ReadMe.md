way to use docker

running docker images docker run -p 8080:8080

build docker:docker build -t springboot-docker-demo .
build docker with version: docker build -t springboot-docker-demo:0.1.RELEASE .

push on docker hub first create repo: docker tag springboot-docker-demo emmizo/springboot-docker-demo:0.1.RELEASE

to push on dockerhub use: docker push emmizo/springboot-docker-demo:0.1.RELEASE

Pull on dockerhub:  docker push emmizo/springboot-docker-demo:0.1.RELEASE

to check list of images: docker images

how to run mysql docker: docker run -p 3307:3306 --name localhost -e MYSQL_ROOT_PASSWORD=Kwizera23 -e MYSQL_DATABASE=blogs -e MYSQL_USER=root -e MYSQL_PASSWORD=Kwizera -d mysql:latest
to start specific docker: docker logs -f dockername

use bash in docker: docker exec -t localhosts bash
