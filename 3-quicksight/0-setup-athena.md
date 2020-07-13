# Set up Athena

1. In the AWS services console, search for **Athena**.

    ![screenshot](../2-athena/img/1.png)

2. If you are using Athena first time, click on “Get Started” button in introduction screen.

    ![screenshot](../2-athena/img/2.png)

3. Athena stores query results in an Amazon S3 bucket and we should configure this before we can explore our dataset. There is already a bucket created for this purpose whose name follows the pattern: `quicksight-lab-data-lake-XXX-YYYY`.

    ![screenshot](../2-athena/img/3.png)

4. To perform such configuration, in Athena Console, click on Settings.

    ![screenshot](../2-athena/img/4.png)

5. Enter bucket name in the query result location field in the following format: `s3://<bucket-name>/` (slashes are important) and click on Save.

    ![screenshot](../2-athena/img/5.png)
