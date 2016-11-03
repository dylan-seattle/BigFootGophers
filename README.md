# GophersLoveAWS
API Challenge for AWS and GO

#API Challenges
===============
API Challenge Challenge Group A

Challenge 1: Write a script that builds three 512 MB EC2 Instances that following a similar naming convention. (ie., web1, web2, web3) and returns the IP of each instance. Use any image you want. Worth 3 Points

Challenge 2: Write a script that snapshots a volume and creates an AMI  (takes an image and deploys the image as a new server with automation). Worth 10 Points

Challenge 3: Write a script that accepts a directory as an argument as well as a  S3 bucket name. The script should upload the contents of the specified directory to the S3 Bucket (or create it if it doesn't exist). The script should handle errors appropriately. (Check for invalid paths, etc.) Worth 5 Points

Challenge 4: Write a script that uses Route 53 to create a new A record when passed a FQDN and IP address as arguments. Worth 3 Points

Challenge 5: Write a script that creates a new DynamoDB database. Should contain at least one database, and the database should have at least one user that can connect to it. Worth 5 Points

##API Challenge Group B
=====================

Challenge 6: Write a script that creates a public S3 website bucket. Must have a index file, error file, and return the status code of a curl test. Worth 10 Points

Challenge 7: Write a script that will create 2 EC2 instances and add them as nodes to a new Elastic Load Balancer. Worth 5 Points


##API Challenge Group C - Tools

Challenge 8: Write an application that when passed the arguments FQDN, image, and flavor it creates a server of the specified image and flavor with the same name as the fqdn, and creates a DNS entry for the fqdn pointing to the server's public IP. Worth 2 Points

Challenge 9: Write an application that will:

Create 2 servers, supplying a ssh key to be installed at /root/.ssh/authorized_keys.
Create a load balancer
Add the 2 new servers to the LB
Set up LB monitor and custom error page.
Create a DNS record based on a FQDN for the LB VIP.
Write the error page html to a file in cloud files for backup.
API Challenge Week 4

Challenge 10: Write an application that will:
Create an SSL terminated load balancer (Create self-signed certificate.)
Create a DNS record that should be pointed to the load balancer.
Create Three servers as nodes behind the LB.
Each server should have a CBS volume attached to it. (Size and type are irrelevant.)
All three servers should have a private Cloud Network shared between them.
Login information to all three servers returned in a readable format as the result of the script, including connection information.
API Challenge Week 5

Challenge 11: Write an application that will
Create a route in mailgun so that when an email is sent to @apichallenges.mailgun.org it calls your Challenge 1 script that builds 3 servers.
Assumptions:
Assume that challenge 1 can be kicked off by accessing http://cldsrvr.com/challenge1
API Challenge Week 6

Challenge 12: Write an application that nukes everything in your Cloud Account. It should:
Delete all Cloud Servers
Delete all Custom Images
Delete all Cloud Files Containers and Objects
Delete all Databases
Delete all Networks
Delete all CBS Volumes
