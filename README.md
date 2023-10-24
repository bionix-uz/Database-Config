### DATABASE (Malumotlar ombori)ni yaratish va configuratsiya qilish.
###### Loyxa uchun PostgreSql DATABASE (Malumotlar obmori) yaratamiz.
``` angular2html
sudo -u postgres psql 
```
``` angular2html
CREATE DATABASE projectname;
```
``` angular2html
 ALTER USER postgres WITH PASSWORD '1'; 
```
``` angular2html 
ALTER ROLE postgres SET client_encoding TO 'utf8';
```
``` angular2html
ALTER ROLE postgres SET default_transaction_isolation TO 'read committed';
```
``` angular2html
ALTER ROLE postgres SET timezone TO 'UTC'; 
```
``` angular2html
GRANT ALL PRIVILEGES ON DATABASE projectname TO postgres;
```
```angular2html
 \q 
```
chiqish uchun.
