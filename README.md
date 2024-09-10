# Getting keys and credentials for running python notebook

Link to dataset: Kaggle dataset: [Stock-market-dataset](https://www.kaggle.com/datasets/jacksoncrow/stock-market-dataset/)

## Getting keys and credentials we'd need for running our notebook

1. **Signing up on AWS**:  Go to [AWS](https://aws.amazon.com/), create an account the proceed to number 2

2. **Creating a User and getting Credentials** : [Watch this youtube video](https://youtu.be/39X5WdZbEwQ?si=FvUMEO2ewe1bU7wS) to get your user credentials using the **IAM** AWS policy. Copy your **Account ID** and **Secret Key** and keep it somewhere, would be used later on

3. **Adding users permissions**: On the page to add the user permissions
![Permissions](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/9b44e3j5h9ejje0px5d0.png)
Add these permissions as seen in the image above:
    - `AmazonS3FullAccess`
    - `AmazonSageMakerFullAccess`
    - `AmazonSNSFullAccess`
    - `AWSBillingReadOnlyAccess`
    - `AWSBudgetsActionsWithAWSResourceControlAccess`
    - `AWSCostAndUsageReportAutomationPolicy`
    - `CloudWatchFullAccess`
4. **Getting account ID**: To get your accont ID, on the drop down like the Image below, copy your Account ID, would be used later on too
    ![Account Id](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/zjvrjmi0kcrlmwievia1.png)

5. **Getting your user region**: On the adding users permissions page, the URL above just like in the image below you can get your `user region`
    ![Get AWS region](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/9r79ti54gws0puv4bgzv.png)
    As seen in the image our region is `eu-north-1`

6. **Using our previous gotten credentials in our code**:
    ![Credentials placeholder](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/8lrwdn5xyk914p72ucly.png)
    In the the third cell in our python notebook, we are to add all our credentials we got preiously to them
    ```python
    AWS_ACCESS_KEY_ID = '' # Secret key
    AWS_SECRET_ACCESS_KEY = '' # Secret Key
    AWS_DEFAULT_REGION = '' # Your AWS region
    MY_EMAIL = '' # Your Email
    ACCOUNT_ID = '' # Your account ID
    ```
    So there we're to add our access key Id, secret access key Id, defalt region, the email you used to signup for AWS and lastly the account ID

7. **Running our code**: Adding all the necessary credentials, create a google colab notebook at [Google Colab](https://colab.research.google.com)
    ![Colab notebook](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/qvydtddoqfufhg9gbwqp.png)

8. **Uploading our notebook**: After creating a new notebook, click on file  then upload notebook to upload our `Cloud_Processing_for_Big_Data.ipynb` notebook to upload our notebook
    ![Upload notebook](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/fftftqdztk5w3d0dg4bd.png)

After uploading notebook, we can now run all our notebook cells


