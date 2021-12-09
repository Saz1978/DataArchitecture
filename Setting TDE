/*this is happening automatically first on master database*/
CREATE MASTER KEY ENCRYPTION BY PASSWORD = 'KEKIC4755Hst57!';

CREATE CERTIFICATE mycert WITH SUBJECT = 'Random Certificate';
/*Switch to the database we want to encrypt this this certificate*/
use SASQLDB;

CREATE DATABASE ENCRYPTION KEY WITH ALGORITHM = AES_256
ENCRYPTION BY SERVER CERTIFICATE mycert;

ALTER DATABASE SASQLDB SET ENCRYPTION ON;
