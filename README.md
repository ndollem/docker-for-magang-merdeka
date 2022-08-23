# Docker sample for Magang Merdeka
Simple Docker compose sample case to setup development environment

## Usefull link for refference

1. https://docs.docker.com/
2. https://docs.docker.com/compose/
3. https://hub.docker.com/

## TODO 

1. Clone it
2. Run `docker-compose up -d` ( `-d` as detach for optional)
3. Create table inside database once you've run the docker container
```sql
drop table if exists `users`;
create table `users` (
    id int not null auto_increment,
    username text not null,
    password text not null,
    primary key (id)
);
insert into `users` (username, password) values
    ("Agus","password"),
    ("Salim","this is my password"),
    ("Salim Agus","this is my second password"),
    ("Agus Salim","p4s5w0Rd"); 
```
