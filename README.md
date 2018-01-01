# docker-run

* zookeeper `docker run --name zookeeper -p 2181:2181 -d zookeeper`
* zookeeper(connect) `docker run --link zookeeper -it --rm zookeeper zkCli.sh -server zookeeper:2181`
* mongodb `docker run --name mongo -p 27017:27017 -d mongo`
* mongodb(connect) `docker run --link mongo -it --rm mongo sh -c 'exec mongo "mongo:27017/test"'`
* mysql `docker run --name mysql -p 3306:3306 -e MYSQL_ALLOW_EMPTY_PASSWORD=1 -d mysql`
* mysql `docker run --link mysql -it --rm mysql mysql -hmysql -uroot`
