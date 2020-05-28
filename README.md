## docker build
<pre>docker build . -t imageName
Ex: docker build . -t teaching-time </pre>

## docker run container
<pre>docker run -p mapPort:portExpose --name nameContainer -t imageName
Ex: docker run -p 8080:8001 --name app-demo -t teaching-time </pre>

## view all container
<pre> docker container ls -a (-s, -l) </pre>

## view image
<pre> docker image ls -abc </pre>

## view all image
<pre> docker images </pre>

## view container runing
<pre>docker ps (-a) </pre>

## remove container
<pre>docker container rm containerName
Ex: docker container rm teaching-time </pre>

## remove image
<pre> docker image rm imageID
Ex: docker image rm abc </pre>

## run docker with image and map to databse
<pre> docker run -p 8090:8090 --name teaching-time --link mysql-standalone -d teaching-time </pre>

## view log docker
<pre> docker logs teaching-time </pre>

## pull phpmyadmin
<pre> docker pull phpmyadmin/phpmyadmin </pre>

## map phpmyadmin to mysql
<pre> docker run -p 6969:80 --name myadmin --link mysql-standalone:db -d phpmyadmin/phpmyadmin </pre>

## login mysql
<pre> mysql -uUsername -pPassword
 mysql -uroot -proot </pre>

## show databse
<pre> show databases; </pre>

## use table
<pre> use tableName </pre>

## show table
<pre> show tables </pre>




