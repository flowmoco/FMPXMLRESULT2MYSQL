FMPXMLResult 2 SQL
==================

The file: FMPXMLRESULT2MYSQL.xslt

This is an XSLT stylesheet that can be used to export data from Filemaker to MySQL

Example use case
---
mysql --user=<\<USERNAME\>> --password=<\<PASSWORD\>> --host=<\<URI\>> --local-infile
LOAD XML LOCAL INFILE "/tmp/table.mysql.xml" INTO TABLE database.table CHARACTER SET \"UTF8\" ROWS IDENTIFIED BY \"\<RECORD\>\"\;
---



FMPXMLResult 2 SQL CREATE TABLE
===============================

The file: FMPXMLRESTULT2SQLCREATETABLE.xslt

This is an XSLT stylesheet that can be used to export table definition from Filemaker to SQL( psql for this one, but can easily be changed to the benefit of MySQL or other SQL dialects )

For now I have not implemented any logic that removes the trailing comma inside the brackets, this may or may not be updated in the future.
