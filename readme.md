## �����Ŀ, ���ɾ���
mvn clean package

## ���� redis
docker run --name redis-server -p 6379:6379 -d redis

## ���� redis-demo
docker run --name redis-demo -p 8080:8080 -d --link redis-server saysky/redis-demo

