# key_rotation_code
Code to receive daily SNS notifications highlighting users with access keys that are over 90 days old

As security best practice AWS recommends that users rotate their access keys every 90 days to decrease the likelihood of accidental exposure, and to protect their AWS resources against unauthorized access.  This code configures a Lambda function to scan your AWS environment for users with access keys that are over 90 days old. We then use EventBridge to trigger the function every 24 hours. SNS then sends an email notification highlighting any out of date access keys.

Access the slide below for a step by step guide 

https://docs.google.com/presentation/d/1xKgy2EqOgW7JISTy0MC-1hKgjv52gThLFffTrlUP2OA/edit?usp=sharing
