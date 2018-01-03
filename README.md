# Message broker RabbitMQ
The RabbitMQ livestream event materials for [pehapkari group](https://github.com/pehapkari)

RabbitMQ basics and examples.

# Requirements
To install [Docker](https://docs.docker.com/engine/installation/#platform-support-matrix)

# Usage
1. run command 
    
    `docker run -d -p 15673:15672 -p 5673:5672 --hostname rabbitmqjb --name rabbitjb rabbitmq:3.6-management-alpine`
    
    1. [RabbitMQ Management console](http://localhost:15673/#/)vám pak bězí na localhost portu 15673
       <http://localhost:15673/#/>
    2. if you want to connect in your application you have to add port number 5673 as you can see in bootstrap.php file

2. run command `composer install` 

## Tip and tricks

`docker system prune` - "clear" your docker local environment

`docker ps` - show all running containers

`docker stop rabbitjb` - stop RabbitMQ instance

`docker restart rabbitjb` - restart RabbitMQ instance
