# CS334DatabaseSystems
repo for cs344 database systems homework - it has the docker files needed for vscode to spin up a docker container containing postresql and mongodb

# to start postgres issue the following command
sudo -i 
su postgres -c '/usr/lib/postgresql/14/bin/pg_ctl start -D /etc/postgresql/14/main'
exit
# note if the above commands fail, use the following commands to reset the permissions on the postgresql folder
sudo -i
chown -R postgres:postgres postgresql/14/main
exit
# then retry starting postgres

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

