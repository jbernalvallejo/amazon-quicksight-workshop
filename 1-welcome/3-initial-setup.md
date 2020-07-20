# Initial Setup

As part of the workshop provisioning, we have taken care of deploying and configuring different resources, that will allow us to consume data from a data lake using Amazon Athena and Amazon QuickSight.

The pipeline deployed looks as follows:

![image](../_media/QuicksightLab.png ':size=750')

1. We provided the data that you will use in QuickSight and is hosted on a S3 bucket. You can go ahead and see it through the Amazon S3 console.
2. We have run a Glue Crawler that discovered the data in S3 and found out the structure. 
3. Once the data was analyzed by AWS Glue, tables were created in the Glue data catalog, ready to be queried.
4. Athena will be used to join different tables and create a view to present the data to Quicksight. You will start the lab by specifying in Amazon Athena where to store the temporary data when submitting the querys. 
5. Then you will move on to the Quicksight console, where you will create an account and get the data from Athena to start creating the Dashboards.
