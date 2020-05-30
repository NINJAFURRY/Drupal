Drupal
Step 1 
Pull imges from docker hub 
#docker pull mysql & docker pull drupal

Step 2
Configure mysql server
#docker run -d -it -e MYSQL_ROOT_PASSWORD=rootpass  -e MYSQL_USER=ninja  -e MYSQL_DATABASE=mydb -v mysql_storage:/var/lib/mysql --nmae dbos mysql:latest

Step 3 
Configure drupal server
#docker run -d -e MYSQL_DATABASE=mydb -e MYSQL_USER=ninja -e MYSQl_PASSWORD=redhat -e MYSQL_ROOT_PASSWORD=redhat drupal:latest

Step 4 
connect to the server
