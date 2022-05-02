# MSCDA_DAP_PROJECT
Sem 1(Python, Data Visualization, Connecting to DB)
Pre-requisite
Please install the following packages

pip install dagster-databricks
pip install psycopg2
pip install dnspython
pip install pymongo
pip install plotly

AWS PostgreSQL DB instance:
Before running the program please start AWS RD **dbinstance-1** below are the login credentials:
URL: https://signin.aws.amazon.com/signin?redirect_uri=https%3A%2F%2Feu-west-1.console.aws.amazon.com%2Frds%2Fhome%3Fregion%3Deu-west-1%26state%3DhashArgs%2523databases%253A%26isauthcode%3Dtrue&client_id=arn%3Aaws%3Aiam%3A%3A015428540659%3Auser%2Frds&forceMobileApp=0&code_challenge=ZCnbim5tla9lh8CfJlsCzlvtePt4yw08bBn6EV-s6D0&code_challenge_method=SHA-256

Username: arpitamitra.16@gmail.com
Password: Password@123
Steps to follow:
select services->Database->RDS->Databases(on left hand side)->dbinstance-1-> Go to Actions dropdown->Select start

MongoDB Connection string: mongodb+srv://DAPProject:Password@dap-cluster.pjiax.mongodb.net/DAP_PROJECT?retryWrites=true&w=majority
User: 'DAPProject'
Password: 'Password'
Database : 'DAP_PROJECT'
If propmpted for ssl please use this string:
client = MongoClient("mongodb+srv://DAPProject:Password@dap-cluster.pjiax.mongodb.net/DAP_PROJECT?retryWrites=true&w=majority",ssl_cert_reqs=ssl.CERT_NONE)


PostgreSQL Connection String: 'postgresql://group_dap123:oYeUKU9ISHQ8@dbinstance-1.c0lqrz3efg7l.eu-west-1.rds.amazonaws.com:5432/DAP'
database='DAP'
user='group_dap123'
password='oYeUKU9ISHQ8'
host='dbinstance-1.c0lqrz3efg7l.eu-west-1.rds.amazonaws.com'
port='5432'

Dataset 1:
The scrapped file from Github has been uploaded in MongoDB. I have then commented out the part of code which is used for uploading the file in MongoDB. 
This has been done to avoid the space issues in database which could arise if the volume of data present in github increases in future.


As the datasets are huge and the results when combined together are very lengthy, we have created four separate blocks of codes to make the dataset-specific charts easily viewable.
