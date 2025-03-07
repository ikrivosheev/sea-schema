# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/)
and this project adheres to [Semantic Versioning](http://semver.org/).

## 0.10.3 - 2022-11-16

* Backward compatible schema discovery for MySQL 5.6 https://github.com/SeaQL/sea-schema/pull/86

## 0.10.2 - 2022-10-26

* Fix parsing of Postgres user-defined types https://github.com/SeaQL/sea-schema/pull/84

## 0.10.1 - 2022-10-23

* Parse & write Postgres array datatypes https://github.com/SeaQL/sea-schema/pull/83

## 0.10.0 - 2022-10-18

* Upgrade SeaQuery to 0.27 https://github.com/SeaQL/sea-schema/pull/81

## 0.9.4 - 2022-09-16

* Parsing SQLite integer column types without space in it https://github.com/SeaQL/sea-schema/pull/77

## 0.9.3 - 2022-07-17

* SQLite real datatype maps to double https://github.com/SeaQL/sea-schema/pull/75
* Discover SYSTEM VERSIONED tables for MariaDB https://github.com/SeaQL/sea-schema/pull/76

## 0.9.2 - 2022-07-04

* PostgreSQL datetime and timestamp datatype are equivalent https://github.com/SeaQL/sea-schema/pull/69
* MySQL VarBinary column type mapping https://github.com/SeaQL/sea-schema/pull/67
* Upgrade `sqlx` to 0.6
* Upgrade `sea-query` to 0.26

## 0.8.1 - 2022-06-17

* Fix SQLx version to ^0.5 https://github.com/SeaQL/sea-schema/pull/70
* PostgreSQL query non-key foreign key info https://github.com/SeaQL/sea-schema/pull/65

## 0.8.0 - 2022-05-09

* Dropping `migration` entirely; introducing `SchemaProbe`

## 0.7.1 - 2022-03-26

* Support SeaORM 0.7.0
* Support Postgres jsonb in entity generation https://github.com/SeaQL/sea-schema/pull/51

## 0.6.0 - 2022-03-14

* Write MySQL unsigned integer types https://github.com/SeaQL/sea-schema/pull/37
* Fix Sqlite BLOB type https://github.com/SeaQL/sea-schema/pull/44
* Migrate with `sea_orm::DbConn` https://github.com/SeaQL/sea-schema/pull/49

## 0.5.1 - 2022-02-07

* Add `migration::prelude` to replace wildcard imports #43

## 0.5.0 - 2022-02-07

* Fix Postgres discover duplicated foreign keys by @billy1624 in https://github.com/SeaQL/sea-schema/pull/30
* Schema Manager by @billy1624 in https://github.com/SeaQL/sea-schema/pull/26

**Full Changelog**: https://github.com/SeaQL/sea-schema/compare/0.4.0...0.5.0

## 0.4.0 - 2021-12-25

* SQLite schema discovery https://github.com/SeaQL/sea-schema/pull/34

## 0.3.1 - 2021-12-12

* Add support for the Postgres interval type by @autarch in https://github.com/SeaQL/sea-schema/pull/20
* CI: Clippy, MySQL & Postgres by @billy1624 in https://github.com/SeaQL/sea-schema/pull/21
* Write MySQL & Postgres Enum Columns by @billy1624 in https://github.com/SeaQL/sea-schema/pull/29

**Full Changelog**: https://github.com/SeaQL/sea-schema/compare/0.2.9...0.3.1

## 0.2.9 - 2021-09-24

+ [[#18]] MySQL: handle panic upon unique constraint

[#18]: https://github.com/SeaQL/sea-schema/issues/18

## 0.2.8 - 2021-09-17

+ Fix Postgres `TimestampWithTimeZone`

## 0.2.7 - 2021-08-23

+ Use SeaRc to support SeaQuery's `thread-safe`

## 0.2.6 - 2021-08-21

+ Use sea-query to 0.15
+ [[#13]] Added `is_identity` to Postgres `ColumnInfo`

[#13]: https://github.com/SeaQL/sea-schema/issues/13

## 0.2.5 - 2021-08-14

+ improve Postgres schema discovery

## 0.2.4 - 2021-08-07

+ improve Postgres schema discovery

## 0.2.3 - 2021-06-19

+ Improve `ColumnType` output of MySQL writer

## 0.2.2 - 2021-06-19

+ Added `ColumnExpression` to MySQL ColumnInfo output
+ Postgres type definitions

## 0.2.1 - 2021-04-30

+ Foreign key writer
+ Index prefix and order

## 0.2.0 - 2021-04-25

+ `Writer`
+ changed `StringAttr` definition
+ added `IndexPart` definition

## 0.1.4 - 2021-04-13

+ serde support on types
+ Query table's `char_set` from information_schema

## 0.1.3 - 2021-04-11

+ `TableInfo` includes `char_set`

## 0.1.2 - 2021-04-11

+ Restructure dependencies

## 0.1.1 - 2021-04-08

+ Fix docs.rs

## 0.1.0 - 2021-04-08

+ Initial release
