# Elastic Cloud Computing (EC2)

**EC2 provides scalable computing capacity in Web Services cloud. Using EC2 eliminates our need to invest in hardware up front, so we can develop and deploy applications faster. we can use  EC2 to launch as many or as few virtual servers as we need, configure security and networking, and manage storage. EC2 enables us to scale up or down to handle changes in requirements or spikes in popularity, reducing our need to forecast traffic.** <br />

#### Amazon EC2 provides the following features:

+ Virtual computing environments, known as instances
+ Preconfigured templates for our instances, known as Amazon Machine Images (AMIs), that package the bits we need for our server (including the operating system and additional software)
+ Various configurations of CPU, memory, storage, and networking capacity for our instances, known as instance types
+ Secure login information for our instances using key pairs (AWS stores the public key, and we store the private key in a secure place)
+ Storage volumes for temporary data that's deleted when we stop or terminate our instance, known as instance store volumes
+ Persistent storage volumes for our data using Amazon Elastic Block Store (Amazon EBS), known as Amazon EBS volumes
+ Multiple physical locations for our resources, such as instances and Amazon EBS volumes, known as Regions and Availability Zones
+ A firewall that enables us to specify the protocols, ports, and source IP ranges that can reach our instances using security groups
+ Virtual networks we can create that are logically isolated from the rest of the AWS cloud, and that we can optionally connect to our own network, known as virtual private clouds (VPCs)