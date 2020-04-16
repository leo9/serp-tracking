# serp-tracking

## to add a new instance:
1. launch from AMI "hdwp"
1. add elastic ip.
1. add elastic ip 27017 to machine "wp1-db & collector & dashboard & backend" security group's import rule.
1. update the instance.json file by adding its instance id to the list. 

## remaining items before launching:
1. Fill in the goldenQuery.json
1. Make capacity number to be 30
1. Add instance id in instance.json (except the 1st one) to lambda function (https://us-west-2.console.aws.amazon.com/lambda/home?region=us-west-2#/functions/bnb_start_stop?tab=configuration) to make it invoked everyday.
1. Launch instance "wp1-db & collector & dashboard & backend" & sudo service mongod start & pm2 start server.js for backend
1. Visit the portal here: http://44.227.79.89/

