# CS334DatabaseSystems
repo for cs344 database systems homework - it has the docker files needed for vscode to spin up a docker container containing postresql and mongodb

# to start postgres issue the following command
su postgres -c '/usr/lib/postgresql/14/bin/pg_ctl start -D /etc/postgresql/14/main'

# to test postgres
su postres
psql
\l
\c mtie
select * from mtie;
\q


# to start mongodb
mongod >> /tmp/mongo.log &

#to test mongo
mongosh
show dbs

