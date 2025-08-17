
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
Click on the 'Workbooks' tab within the Log Analytics Workspace. Select 'Add new' to create a new workbook. Once inside the workbook editor, navigate to the 'Advanced Editor' section and input the appropriate Kusto Query Language (KQL) script to generate the desired map visualization.

<img width="929" height="415" alt="brave_BwJdhCo4oY" src="https://github.com/user-attachments/assets/125f3c10-3095-498a-9fb6-f44002b5797a" />

<img width="1258" height="713" alt="brave_SrTv3vOQba" src="https://github.com/user-attachments/assets/f35461e7-3ed3-406d-a823-d8cbfc809262" />


### File Share Setup
