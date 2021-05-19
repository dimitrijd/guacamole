10007  docker pull guacamole/guacamole
10008  docker pull guacamole/guacd

supporting service running on docker's port 4822 (it must be linked) 
10009  docker run --name guaca -d guacamole/guacd

generating DB script
10011  docker run --rm guacamole/guacamole /opt/guacamole/bin/initdb.sh --mysql > initdb.sql

mysql
10015  docker pull mysql
docker run --name guaca-db -e MYSQL_ROOT_PASSWORD=pass -d mysql
