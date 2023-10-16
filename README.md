# Cryptoaddik
Cold Storage for Bitcoin and other Cryptocurrencies

Notice of Copyrights and Licenses:
---------------------------------------
The addik.co project, software and embedded resources are copyright addik.co.

The addik.co name and logo are not part of the open source license.

Requires
---------------------------------------
Minimum Xojo 2018r1.1

Any SQLite Manager (with encryption capability)

Summary of licenses needed:

The MBS Xojo Barcode Plugin - Get it at: https://www.monkeybreadsoftware.de/xojo/plugin-barcode.shtml

The MBS Xojo Encryption Plugin - Get it at: https://www.monkeybreadsoftware.de/xojo/plugin-encryption.shtml

Chilkat Xojo Plugin - Get it at: https://www.chilkatsoft.com/xojo.asp

Create SQLite database name dummy.dat with the 2 tables below
---------------------------------------
```
CREATE TABLE [Addresses] (AID integer NOT NULL PRIMARY KEY AUTOINCREMENT,address varchar,private varchar,compress integer,date integer,type integer,amount integer NOT NULL DEFAULT 0,status integer NOT NULL DEFAULT 0,ticker varchar,coin varchar)
```
```
CREATE TABLE [User] (ID integer NOT NULL PRIMARY KEY AUTOINCREMENT,encryp varchar,date integer,version varchar,status integer NOT NULL DEFAULT 0,datav varchar,lastcomp integer NOT NULL DEFAULT 0,lastp integer NOT NULL DEFAULT 5,spare1 varchar,lastcoin varchar NOT NULL DEFAULT Bitcoin,pick integer NOT NULL DEFAULT 0)
```
