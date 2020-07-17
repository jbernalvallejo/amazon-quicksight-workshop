# Initial Setup

These are the different services and steps that happened for you to be able to do this workshop

![image](../_media/QuicksightLab.png ':size=750')

This is what happened and was provided to you behind the scenes:

1. We provided the data that you will use in quicksight and is on a S3 bucket, you can go ahead a see it
2. We have run a glue crawler that discovered the data and found out its structures 
3. Now that the data was analyzed by glue it create a table in the data catalog
4. With Athena we will do for you a join of the different tables and create a view to present the data to Quicksight, You will start the lab specifying to athena where to store the temporary data when submitting the querys 
5. Then you will move on to Quicksight create an account and get the data from Athena to create your Dashbords.
