# Regions and availability Zones

## Regions 
AWS has the concept of a region, which is a physical location, somewhere in the world, where they put their data centers. which have the servers that host all of their services. currently, AWS has regions in North America, South America, Europe, the middle East, Africa, Asia Pacific, Canada Central, Canada West.

| Region Name             | Region     |
|-------------------------|------------|
| US East (Ohio)          | us-east-2  |
| US East (N. Virginia)   | us-east-1  |
| US West (N. California) | us-west-1  |
| US West (Oregon)        | us-west-2  |
| Africa (Cape Town)      | af-south-1 |
| Asia Pacific (Hong Kong)| ap-east-1  |
| Asia Pacific (Hyderabad)| ap-south-2 |
| Asia Pacific (Jakarta)  | ap-southeast-3 |
| Asia Pacific (Melbourne)| ap-southeast-4 |
| Asia Pacific (Mumbai)   | ap-south-1 |
| Asia Pacific (Osaka)    | ap-northeast-3 |
| Asia Pacific (Seoul)    | ap-northeast-2 |
| Asia Pacific (Singapore)| ap-southeast-1 |
| Asia Pacific (Sydney)   | ap-southeast-2 |
| Asia Pacific (Tokyo)    | ap-northeast-1 |
| Canada (Central)        | ca-central-1 |
| Canada West (Calgary)   | ca-west-1   |
| Europe (Frankfurt)      | eu-central-1 |
| Europe (Ireland)        | eu-west-1   |
| Europe (London)         | eu-west-2   |
| Europe (Milan)          | eu-south-1  |
| Europe (Paris)          | eu-west-3   |
| Europe (Spain)          | eu-south-2  |
| Europe (Stockholm)      | eu-north-1  |
| Europe (Zurich)         | eu-central-2 |
| Israel (Tel Aviv)       | il-central-1 |
| Middle East (Bahrain)   | me-south-1  |
| Middle East (UAE)       | me-central-1 |
| South America (São Paulo)| sa-east-1  |
| AWS GovCloud (US-East)  | us-gov-east-1 |
| AWS GovCloud (US-West)  | us-gov-west-1 |




## Availability Zones 

Inside region AWS has Availability zones.

Each region has multiple isolated and physically separate availability zones in a geographic area. they all have independent power, cooling annd physical security, and they are all connected to each other via redundant ultraa high speed, and low latency networks. 

So let's say in the Sydney region which is `ap-aoutheast-2` aws has 6 datacenter around the city. AWS groups them into  north, south and west availability zones. and will give them each a name, but these names are not shared between users or AWS accounts. 

For example in my account, I will have the West availability zone called ap-southeast-2a  north will be 2b and south will be 2c. But in your account, this won't be the same. It's possible it could be the same, but they are randomly generated. So in your account you will be ap-southeast-2c in the west, 2a in the north and 2b in south.

This occurs in every availability zone around the world to ensure that people aren't always just using availability zone a or b for their infrastructure. They want everything spreadout across all of their availability zones. 

**What's the purpose of having these availability zones?**   
Well redundancy, If you split your aws services across all of these availability zones, you will protect your AWS workloadd from any issues that might arise in a single data center. It's unlikely that all six of these data centers will lose power at the same time. or be hit with any kind of local infrastructure issue. 