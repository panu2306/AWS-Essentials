### AWS Regions & Availibility Zones: 

Amazon EC2 is hosted in multiple locations world-wide. These locations are composed of regions & each region has multiple availability zones which are physical data centres. For example, `us-east-1` is the region & `us-east-1a` is the availibility zone for that region. Each region can have multiple availibility zones. To differentiante one availibility zone from other AWS can use letters from `a-z` for identifying availibility zones. For more information please head to [AWS regions & availibility zones](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-regions-availability-zones.html).

Another one concept is local zone. Local zones are the regions which are close to the user. Always select region that is closer to you for faster access to your EC2 instance. Also, note that not all the regions support local zones. We need to check if that region supports for local zones. For more information please head to [available regions](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-regions-availability-zones.html#concepts-available-regions).

### Security Groups
Security Gropus are fundamental of network security in AWS. They control how the traffic is allowed into or out of our EC2 Machines. Security groups comes in between the EC2 Machine & user(browser or terminal). 

When we launch an EC2 instance we can assign upto five security groups to that instance. Security group act an the instance level so every other instance in you VPC can have different security group. 

For each security group you can have different set of rules to control the inbound traffice as well another different set of rules to control the outbound traffic. 

To know more about security groups for linux instances click to [this](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-security-groups.html).







