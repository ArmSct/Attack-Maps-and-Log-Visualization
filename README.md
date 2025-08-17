
<img width="723" height="259" alt="image" src="https://github.com/user-attachments/assets/ff8c0f1c-362a-468d-a74c-47c0bbbb6c07" />


# Attack Maps and Log Visualization
In this project I use all the logs being created within the environment (some frome students, some from bad actors on the internet) to create world map visualization workbooks for various scenarios based on originating IP address just to give a visualization of what’s happening in the network.

All relevant logs from network devices, servers, and applications will be systematically collected and forwarded to Microsoft Sentinel (SIEM).

<img width="1188" height="573" alt="brave_3pi3aO8Koy" src="https://github.com/user-attachments/assets/20af3788-9e8c-454d-ba88-38f741276dd9" />


## Technologies Utilized
- Microsoft Azure (Virtual Machine deployment)
- Microsoft Sentinel (SIEM)
- Kusto Query Language (KQL) 
- Windows 10

## Actions and Observations

### Azure Portal
Access the Microsoft Azure Portal and authenticate using your organizational credentials. From the portal homepage, proceed to the Microsoft Sentinel service. Within the Sentinel interface, Open the linked Log Analytics Workspace.

<img width="794" height="370" alt="brave_I2dF81UvI7" src="https://github.com/user-attachments/assets/bb061255-109e-4692-b3a1-6c58274414db" />

<img width="732" height="415" alt="brave_janWhZBusl" src="https://github.com/user-attachments/assets/6b0c59f0-8967-49d6-bdb1-7c71ebfc5a8f" />

### Workbook
Click on the 'Workbooks' tab within the Log Analytics Workspace. Select 'Add new' to create a new workbook. 
<img width="929" height="415" alt="brave_BwJdhCo4oY" src="https://github.com/user-attachments/assets/125f3c10-3095-498a-9fb6-f44002b5797a" />

Once inside the workbook editor, navigate to the 'Advanced Editor' section and input the appropriate Kusto Query Language (KQL) script to generate the desired map visualization.
<img width="1258" height="713" alt="brave_SrTv3vOQba" src="https://github.com/user-attachments/assets/f35461e7-3ed3-406d-a823-d8cbfc809262" />

## Maps

### Entra ID (Azure) Authentication Success
This map is a visual representation of successful login attempts to your Azure environment (tenant-wide) from users across different geographic locations. The size and color of the marker indicate the number of successful logins. The more logins there are from a location, the larger and redder the marker appears on the map, while fewer logins result in a smaller, greener marker.

<img width="927" height="668" alt="brave_CymVKsIAyK" src="https://github.com/user-attachments/assets/6fd9c055-a18a-4c5f-838d-2b60005eecc5" />

### Entra ID (Azure) Authentication Failures
This map shows where in the world users are failing to log in to the Azure tenant, based on unsuccessful authentication attempts recorded in the SignInLogs table. Green markers indicate fewer failures, while red markers indicate a higher volume of failures.

<img width="935" height="670" alt="brave_VMnv9JCHSi" src="https://github.com/user-attachments/assets/3ea014fd-4b8c-4840-8fd9-86de63ac4c2d" />

### Azure Resource Creation
This map shows who created Azure resources, from where, and how many resources they created, based on logs collected in the Azure Activity Log. The colors represent the number of resources created from each location. Green indicates low activity (fewer resources created) and red highlights the locations with the highest number of resource creations.

<img width="922" height="635" alt="brave_ddu6DGHqxf" src="https://github.com/user-attachments/assets/fd914e02-68c7-4d29-9c3d-d7fd55c9e44a" />

### VM Authentication Failures
This map is a visual representation of failed login attempts across all virtual machines onboarded to Microsoft Defender for Endpoint in your tenant. The map’s colors show the number of failed login attempts, with red or darker colors indicating more failures and lighter colors indicating fewer.

<img width="920" height="665" alt="brave_ZznVzzBBzR" src="https://github.com/user-attachments/assets/82c9edfd-8b17-4d70-bdc3-a6dba2e26073" />

### Malicious Traffic Entering the Network
This map visualizes the inbound network traffic that has been flagged as malicious by Microsoft’s threat intelligence. The markers on the map represent the geographic locations of IP addresses that have sent malicious traffic into the network. Intense or warmer colors (like red or orange) indicate a higher number of or more severe threats, while cooler colors (like blue or green) represents fewer or less severe malicious events.

<img width="920" height="662" alt="brave_0AKUHLG5pf" src="https://github.com/user-attachments/assets/5fadf2d0-2344-4310-8f63-79c720ecde40" />

