# flyway-issue-7685 project

This project is about to reproduce the flyway exceptions while deployed native way.

it works while ```mvn quarkus:dev```


## Pre-steps

### Replace the mysql db host name and credentials in application.properties

### Create the databases;
```sh
create database db1;
create database db2;
```

### Reproduce
```sh
mvn clean package -Pnative

./target/flyway-issue-7685-1.0-SNAPSHOT-runner

```