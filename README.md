# PostgreSQL Database Interface for VeighNa Framework

<p align="center">
  <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
</p>

<p align="center">
    <img src ="https://img.shields.io/badge/version-1.0.1-blueviolet.svg"/>
    <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
    <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
</p>

## Description

Based on the PostgreSQL database interface developed by peewee.

## Use

### Global Configuration

To use PostgreSQL in VeighNa, you need to fill in the following field information in the global configuration:

|name|meaning|required|examples|
|---------|----|---|---|
|database.name|Name|Yes|postgresql|
|database.host|Address|Yes|localhost|
|database.port|Port|Yes|5432|
|database.database|Instance|Yes|vnpy|
|database.user|Username|Yes|postgres|
|database.password|Password|Yes|123456|

Please note that VeighNa does not actively create databases for relational databases, so please make sure that the database corresponding to the database.database field you filled in has been created. If no database has been created, please connect to it manually and create it.

### Creating an instance

VeighNa does not create instances of PostgreSQL databases on its own initiative, so please make sure that the instance of the database you filled in the database.database field has been created before using it.

If an instance has not been created, you can use [Create Database] in the [pgAdmin 4] client.