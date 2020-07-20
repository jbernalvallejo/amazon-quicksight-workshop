# Set up QuickSight

1.	In the AWS services console, search for QuickSight.

    ![screenshot](img/1.png)

If this is the first time you have used QuickSight, you are prompted to create an account. 

2.	Click Sign up for QuickSight.

    ![screenshot](img/2.png)

3.	For account type, please choose Enterprise Version.

    ![screenshot](img/3.png)

4.	Click Continue.

5.	On the Create your QuickSight account page, under the QuickSight region section,  **select EU (Ireland) region**, accept the warning by clicking OK.

    ![screenshot](img/4.png)

6.  Scroll down and set a name for the account and type an email address.

7.	Ensure "Enable autodiscovery of data" and "Amazon Athena" are selected.

8.	Click on "Amazon S3" and select the two available buckets starting with `quicksight-lab-`.

    ![screenshot](img/5.png)

    ![screenshot](img/6.png)

9.	Click Finish. It will take some time for the new account to be created. Once it is done, go to the Amazon Quicksight dashboard.

10.	We are going to configure now the data set for the Quicksight analysis/dashboard that we will be building based on one of the Athena views that were created automatically for the AWS account you are using. In order to do that, click Manage Data on the top right corner.

    ![screenshot](img/7.png)

11.	Click New Dataset.

    ![screenshot](img/8.png)

12.	On the Create a Data Set page, select Athena as the data source.

    ![screenshot](img/9.png)

13.	For Data source name, type `ticketdata-qs` and click Validate connection.

14.	Once validated, click Create data source.

    ![screenshot](img/10.png)

15.	In the database drop-down list, select “ticketdata” database.

16.	Choose the "sporting_event_ticket_info" table and click Select.

    ![screenshot](img/11.png)

17.	To finish data set creation, choose the option Import to SPICE for quicker analytics and click Visualize.

    ![screenshot](img/12.png)

    > [!NOTE]
    > SPICE is an in-memory-calculation engine that enables achieving fast performance at scale. Data is automatically replicated for high availability allowing thousands of users to simultaneously perform fast, interactive analysis while shielding your underlying data infrastructure, saving you time and resources. This lab account has been created with a default SPICE size of 1GB. If needed, it could be increased Quicksight account settings.

You will now be taken to the QuickSight Visualize interface where you can start building your dashboard.  

![screenshot](img/13.png)

> [!NOTE]
> The SPICE dataset will take a few minutes to be built, but you can continue to create some charts on the underlying data.
