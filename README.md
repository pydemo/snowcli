# snowcli
Snowflake DB SQL shell/cli



## Set environment for pyodbc

```
export SNOWFLAKE_ROLE=my_role
export SNOWFLAKE_SERVER=MYDATAART
export SNOWFLAKE_WSID=my-wsid
export SNOWFLAKE_AUTOCOMMIT=False
export SNOWFLAKE_WAREHOUSE=MYWH
export SNOWFLAKE_APP=MYAPP
export SNOWFLAKE_DATABASE=MYDB
export SNOWFLAKE_SCHEMA=MYSCHEMA
export SNOWFLAKE_USER=dev_test
export SNOWFLAKE_PWD=mypwd
export SNOWFLAKE_AUTHENTICATOR=https://test.okta.com;uid=dev-testt@test.com
```

## Cli entry


```
host:/home/user/snowcli $ ~/python3/bin/python3 main.py 
Snow>
```

##Load file into Snowflake table.

```
Snow> COPY INTO MYDB.MYSCHEMA.MY_TABLE FROM '@MY_STAGE/MY_TABLE/'FILES=('test.csv.gz') 
```

![Screenshot](https://raw.githubusercontent.com/pydemo/snowcli/master/snowcli2.PNG)


### Other scrips

https://github.com/pydemo/s3cli



