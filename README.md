# ODTP
Oracle data to PostgreSQL (ODTP)


1. Assume that tables in PG and Ora has same structure.
2. Table structure migrate recommend use Ora2pg
3. Foreign Key need to disable while migrate data, this tool not deal with the FK
4. Oracle need to support partition table
5. Using multi thread to migrate data to reduce migrate time<br/>
   a. Table rows which less than 500,000 will migrate data directly<br/>
   b. Table rows which bigger than 500,000 will divide into multi bucket<br/>
6. This tool read data from Oracle then insert into PG, no stage data will be generate
