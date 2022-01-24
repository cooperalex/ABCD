
# Install Postgres on Ubuntu

`$ sudo sh -c 'echo "deb http://apt.postgresql.org/pub/repos/apt $(lsb_release -cs)-pgdg main" > /etc/apt/sources.list.d/pgdg.list'`

`$ wget --quiet -O - https://www.postgresql.org/media/keys/ACCC4CF8.asc | sudo apt-key add -'`

`$ sudo apt-get update`

`$ sudo apt-get install postgresql-14`

`$ sudo systemctl enable postgresql`

`$ sudo 


`$ sudo -i -u postgres`

`$ psql`

`create user user  abcd;`

`alter user  abcd   password "abcd";`

`quit`

`createdb -D abcd -O abcd -U abcd`

`$ createdb -O abcd abcd` 