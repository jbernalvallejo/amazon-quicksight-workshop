# Initial Setup

These are the different services and steps that happened for you to be able to do this workshop

![image](../_media/QuicksightLab.png ':size=750')

This is what happened and was provided to you behind the scenes

1. We provided the data that you will use in quicksight and is on a S3 bucket, you can go ahead a see it
2. We have run a glue crawler that discovered the data and found out its structures 
3. Now that the data was analyzed by glue it create a table in the data catalog
4. You will start the lab creating views that will perform the joins between the tables to present the data to Quicksight via Athena
5. Quicksight gets the data from Athena and you can create your Dashbords.
