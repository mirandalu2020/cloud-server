# cloud-server
Deploy a simple Node.js server to EC2, using Elastic Beanstalk

## URL

[aws-practice](http://awsdeploy-env.eba-avcmfcpg.us-east-1.elasticbeanstalk.com/)

[message-me](http://lab-env.eba-npejgmuu.us-west-2.elasticbeanstalk.com/)

## Process

### using the AWS GUI

1. zip the folder of interest, make sure zip the contents only NOT the folder
2. use command `zip -r <aws.zip> </source/*>
3. upload the zip file on the Elastic Beanstalk console
4. **IT WILL FAIL!** Change the bucket permission to allow ALC
5. Re-upload and deploy

### using EB-CLI

1. cd into the repo locally
2. type `aws configure`, type in user id and secret
3. `eb init`, no awscommit
4. `eb create <env-name-env>`
5. `eb deploy` (say yay!)
6. the application should show up on the elastic beanstalk dashboard, DOUBLE CHECK THE REGION
