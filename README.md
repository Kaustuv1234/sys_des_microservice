# sys_des_microservice

![alt text](https://github.com/Kaustuv1234/sys_des_microservice/blob/main/diagram.png?raw=true)

tutorial: https://www.youtube.com/watch?v=hmkF77F9TLw&t=435s

for importing in server.py: ```pip install jedi pylint pyjwt flask ```

```brew install mysql-client pkg-config```

```export PKG_CONFIG_PATH="/opt/homebrew/opt/mysql-client/lib/pkgconfig"```

```pip install flask_mysqldb```

```export MYSQL_HOST=localhost```

after writing init.sql file - ```mysql -uroot < init.sql```

to open mysql - ```mysql -uroot```

to see databases - ```show databases;```

open auth db - ```use auth;```

see tables - ```show tables;```

check user table - ```describe user;``` and then ```select * from user;```


after writing Dockerfile - ```docker build -t auth_latest .```

Note: in manifests we are using the image ```sweasytech/auth``` not the image we created

after writing manifest files - ```kubectl apply -f ./```, then ```k9s``` to see 2 instances running

inside k9s press enter on a container and then 's' to use the shell inside the container