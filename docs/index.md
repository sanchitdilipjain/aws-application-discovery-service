## AWS Application Discovery Service

<meta name="image" property="og:image" content="images/image1.png">
<meta property="og:image:height" content="150">
<meta property="og:image:width" content="300">

**Introduction**

- AWS Discovery Agent is an AWS software that is deployed in any targeted servers like physical on-premises servers, Amazon EC2 instances, and virtual machines for discovery and migration. It captures information like system configuration, system performance, running processes, and details of the network connections between systems.

- This agent required root privileges to collect the information. When you start the Discovery Agent, it registers with the Application Discovery Service endpoint, arsenal.aws.com, and pings the service at 15-minute intervals for configuration information

- To initiate the agent to capture data collection we need to send a command. All the information captured helps to visualize all the IT assets and their dependencies, calculate the total cost of ownership, and also the migration plan.

- Data captured is transferred securely using Transport Layer Security (TLS) encryption. Agents are configured to upgrade automatically when new versions become available. You can change this configuration setting if desired.

  <p align="center"><img src="images/image1.png" class="inline" width="500" height="150"/></p>

**Tutorial**

- On this section we will start utilizing AWS Application discovery services, by:

  - Create AWS Credentials  
  
  - Installing ADS agents in the servers
  
  - Starting ADS data collection
  
  - Browsing the discovered data
  
  - Viewing Network Connections
  
  - Explore EC2 instance recommendations
  
  - Enabling ADS and Athena integration

- Create AWS Credentials 

  1. Traverse to the <a href="https://console.aws.amazon.com/iamv2/">Amazon IAM console</a>  
  
  2. In the IAM screen, click on Users and Select Add users button on the right side of the screen
  
      <p align="center"><img src="images/image2.png" class="inline" width="700" height="125"/></p>
  
  3. Provide Username ADSAgent and select Programmatic access under Access type
      
      <p align="center"><img src="images/image3.png" class="inline" width="700" height="400"/></p>
  
  4. Click Next to add required permission. Under permission screen, choose Attach existing policies directly and select AdministratorAccess under Poilcy Name
  
      <p align="center"><img src="images/image4.png" class="inline" width="700" height="400"/></p>
  
  5. Click Next, and provide required tags
  
  6. Click Next, and review all the provided details. Finally click Create user
  
      <p align="center"><img src="images/image5.png" class="inline" width="700" height="400"/></p>
  
  7. Now the user is created, download the csv file which contains Access & Secret Key required while deployed AWS Discovery Agent
  
      <p align="center"><img src="images/image6.png" class="inline" width="700" height="350"/></p>

- Installing ADS agents in the servers

- Starting ADS data collection

- Browsing the discovered data

- Viewing Network Connections

- Explore EC2 instance recommendations

- Enabling ADS and Athena integration
