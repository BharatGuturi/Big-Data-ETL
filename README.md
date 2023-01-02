# Big-Data-ETL
To perform the ETL process completely in the cloud and upload a DataFrame to an RDS instance. 

# Instructions
1)  To execute the project follow the below commands: git clone https://github.com/BharatGuturi/Big-Data-ETL.git

2)  Create an AWS account.

3)  Create RDS and S3 in AWS.

3)  Connect google colab with the ipynb files.

4) S3 bucket setting:
    {
    "Version": "2012-10-17",  
    "Statement": [  
        {  
            "Sid": "getobject",  
            "Effect": "Allow",  
            "Principal": "*",  
            "Action": "s3:GetObject",  
            "Resource": "<bucket codes>/*"  
          }
      ]
  }

5)  Install the required libraries using the following commands: 
    pip install pypandoc
    pip install pyspark
    
6) In the following command in the 'Load' section, use the endpoint created in AWS in <endpoint> and database name in <database_name>. In the config command, use the username and password used to create the database
 
    jdbc_url="jdbc:postgresql://<endpoint>:5432/<database_name>" 
    
    config = {"user":"", "password": "", "driver":"org.postgresql.Driver"}
    
Run the "Unsupervised Machine Learning.ipynb" file
