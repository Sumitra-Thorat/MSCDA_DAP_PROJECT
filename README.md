# MSCDA_DAP_PROJECT
Sem 1(Python, Data Visualization, Connecting to DB)
Pre-requisite
Please install the following packages

pip install dagster-databricks
pip install psycopg2
pip install dnspython
pip install pymongo
pip install plotly

MongoDB Connection string: mongodb+srv://DAPProject:Password@dap-cluster.pjiax.mongodb.net/DAP_PROJECT?retryWrites=true&w=majority
User: 'DAPProject'
Password: 'Password'
Database : 'DAP_PROJECT'
If propmpted for ssl please use this string:
client = MongoClient("mongodb+srv://DAPProject:Password@dap-cluster.pjiax.mongodb.net/DAP_PROJECT?retryWrites=true&w=majority",ssl_cert_reqs=ssl.CERT_NONE)

AWS PostgreSQL DB instance: dbinstance-1
PostgreSQL Connection String: 'postgresql://group_dap123:oYeUKU9ISHQ8@dbinstance-1.c0lqrz3efg7l.eu-west-1.rds.amazonaws.com:5432/DAP'
database='DAP'
user='group_dap123'
password='oYeUKU9ISHQ8'
host='dbinstance-1.c0lqrz3efg7l.eu-west-1.rds.amazonaws.com'
port='5432'

Dataset 1:
The scrapped file from Github has been uploaded in MongoDB. I have then commented out the part of code which is used for uploading the file in MongoDB. 
This has been done to avoid the space issues in database which could arise if the volume of data present in github increases in future.
