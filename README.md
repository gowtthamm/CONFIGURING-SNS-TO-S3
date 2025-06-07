# Configuring-SNS---S3-Practice

<img src="https://github.com/gowtthamm/Configuring-SNS---S3-Practice/blob/0d892994f71686de97a779dfe4d633942bec1c6e/SNS%20to%20S3.jpeg" width="500" height="500" />

PROCEDURE:
01.	Create Topic and add Subscription Inside  the Topic  : TOPIC  ARN  = Task
02.	Select The Portal  :  Email ¬ - Enter Your Mail and Click Create Subscription 

<img src="https://github.com/gowtthamm/Configuring-SNS---S3-Practice/blob/60fbede38a61a78fa57f92c0ce5a48b4c9501379/EMAIL.png"/>

03.	Now Create One Simple Normal S3 Bucket  :  gowthamnotification

<img src="https://github.com/gowtthamm/Configuring-SNS---S3-Practice/blob/4f2668619fc91694c9f10fee52a8a0e711a437d6/Notification.png"/>

04.	Now Configure SNS To S3 (Task – gowthamnotification  )
05.	Go to SNS : Topic – select Task – Access Policy  (Edit) – Clear  Existing Code and add this :-

 https://github.com/gowtthamm/Configuring-SNS---S3-Practice/blob/5131396b5020e8c576b7c45fab9f9b22d3b1319b/JSON%20%20Code

06. Copy and Paste The ARN ID  in  ( "Resource": "SNS-topic-ARN", )

<img src="https://github.com/gowtthamm/Configuring-SNS---S3-Practice/blob/aed05927b098519caa191bf7c9dc8994d10db43f/ARN.png"/>

07. 07.	Same, Copy and paste The Bucket Name  in ("aws:SourceArn": "arn:aws:s3:*:*:bucket-name")
08.	Same that Copy and Paste The Owner ID in ("aws:SourceAccount": "bucket-owner-account-id")
09.	Click  Save Changes 
10.	Now , Go to S3 Bucket (gowthamnotification) -  Properties  - Event Notification




