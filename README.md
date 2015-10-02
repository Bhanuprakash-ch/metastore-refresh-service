[![Code Climate](https://codeclimate.com/github/trustedanalytics/metastore-refresh-service/badges/gpa.svg)](https://codeclimate.com/github/trustedanalytics/metastore-refresh-service)

# metastore-refresh-service
Service for refreshing metastore data about tables for Impala

## REST endpoints

Table names can contain database prefix. So **default.table** is accepted by the service

* **/api/spec** returns API specification
* **/** returns status message
* **/refresh/<table_name>** refreshes single table
* **/invalidate/** invalidates whole metastore
* **/invalidate/<table_name>** invalidates data related to only one table

