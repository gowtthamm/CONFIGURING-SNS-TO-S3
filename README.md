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



06. Copy and Paste The ARN ID  in  ( "Resource": "SNS-topic-ARN", )


