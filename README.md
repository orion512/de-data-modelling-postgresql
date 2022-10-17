# Data Modelling with PostgreSQL

This repository serves as a submission for Udacity data engineer nanodegree.




## Helper Commands for postgreSQL

**login to psql with {postgres} user**
```
# linux
sudo -u {postgres} psql

# windows
psql -U postgres
```

**PSQL commands**
```
\conninfo # connection info
\l # list all databaes
\dt # list all relations
\du # list all users
CREATE USER <username> WITH PASSWORD '<password>';
CREATE DATABASE <name> WITH OWNER <username>;
GRANT ALL PRIVILEGES ON DATABASE db_name to user_name;
ALTER USER username CREATEDB; # grant user privilege to create dbs
```

**reinstall pgsql DB**
```
# linux
sudo yum remove postgresql11-server

sudo rm -rf  /var/lib/pgsql/11/data
sudo /usr/pgsql-11/bin/postgresql-11-setup initdb

sudo systemctl start postgresql-11
sudo systemctl enable postgresql-11

sudo systemctl restart postgresql-11 # restart service
```
