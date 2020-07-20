# Set up Athena

1. In the AWS services console, search for **S3**.

    ![screenshot](../2-athena/img/openS3.png)

2. Select the bucket `quicksight-lab-athena-results-<region>-<account-id>`.

    ![screenshot](../2-athena/img/selectbucket.png)

3. Copy the name from the bar on top.

    ![screenshot](../2-athena/img/copybucketname.png)

4. From services on top type and select Athena.

    ![screenshot](../2-athena/img/gotoathena.png)


5. If you are using Athena for the first time, click on “Get Started” button in the introduction screen.

    ![screenshot](../2-athena/img/2.png)

6. Athena stores query results in an Amazon S3 bucket and we should configure this before we can explore our dataset. There is already a bucket created for this purpose whose name follows the pattern: `quicksight-lab-athena-results-<region>-<account-id>`. You should have it on your clipboard as per the step above.

    ![screenshot](../2-athena/img/3.png)

7. To perform such configuration, in Athena Console, click on Settings.

    ![screenshot](../2-athena/img/4.png)

8. Enter bucket name in the query result location field in the following format: `s3://quicksight-lab-athena-results-<region>-<account-id>/` use the name you copied from the bucket in S3 (slashes are important) and click on Save.

    ![screenshot](../2-athena/img/5.png)
