#docker build
docker build . -t <image name>
Ex: docker build . -t <teaching-time>

#view all container
docker container ls -a (-s, -l)

#view image
docker image ls -abc

#view container runing
docker ps (-a)

#remove container
docker container rm <container name>
Ex: docker container rm teaching-time

#remove image
<pre> docker image rm <image id>
Ex: docker image rm abc </pre>

#run docker with image and map to databse
<pre> docker run -p 8090:8090 --name teaching-time --link mysql-standalone -d teaching-time </pre>

#view log docker
<pre> docker logs teaching-time </pre>

#pull phpmyadmin
<pre> docker pull phpmyadmin/phpmyadmin </pre>

#map phpmyadmin to mysql
<pre> docker run -p 6969:80 --name myadmin --link mysql-standalone:db -d phpmyadmin/phpmyadmin </pre>

#login mysql
<pre> mysql -u<username> -p<password>
mysql -uroot -proot </pre>

#show databse
<pre> show databases; </pre>

#use table
<pre> use <table name> </pre>

#show table
<pre> show tables </pre>




