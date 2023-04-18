# Crowd Strike Filevantage API connector for QRadar

# How to Generate Crowd Strike Filevantage API token
1. Log on to your Falcon UI.

2. navigate to Support > API Clients and Keys.

3. In the Admin Configuration press at API Management.

4. Press "add new API" button and you will be prompted to give a descriptive name and select the appropriate API scopes.

5. After you click save, you will be presented with the Client ID and Client Secret. The secret will only be shown once and should be stored in a secure place.


# QRadar Log Source Configuration
A workflow XML document defines the behavior of the Universal Cloud REST API protocol. To ingest data from an endpoint through the Universal REST API protocol, you can create a log source on the QRadar® Console using the Log Source Management app. In the Workflow field of the log source, you can specify how the endpoint can communicate with QRadar using the Universal REST API protocol.

The parameters XML document specifies the user settings for this log source, including API authentication and relevant configurations.

1. Log in to QRadar and click the admin panel.

2. To create DSM, click the DSM editor app icon.

3. Then click Create New and insert the name (_Crowd Strike Filevantage API_).

4. To create the log source, go to admin panel and click the QRadar Log Source Management app icon.

5. Click New Log Source > Single Log Source.

6. On the Select a Log Source Type page, Select a Log Source Type Crowd Strike Filevantage API.

7. On the Select Protocol Type page, select Universal Cloud REST API, and go to Step 3.

8. On the Configure the Log Source parameters page, configure the log source name and click Configure Protocol Parameters. 

9. On the Configure the Protocol Parameters page, configure the protocol-specific parameters:
 - Insert a log source identifier (Crowd_Strike_Filevantage_API);
 - Copy the Workflow XML you downloaded from GitHub and paste it into the Workflow field;
 - Copy the Workflow Params (make sure your api_host, client_id and client_secret are populated) into the Workflow Parameters Values field;
 - **Make sure to turn off the Coalescing Events to avoid grouping of the events on the basis of Source and Destination IP.**

10. In the Test protocol parameters window, click Start Test.

10. To fix any errors, click Configure Protocol Parameters. Configure the parameters and click Test Protocol Parameters.

11. Click Finish
# Crowd Strike Filevantage Parameters Configuration
Parameter           |   Name    |   Default Value |   Type    |   Required (True/False)   |   Description
---                                 | --- | --- | --- |--- |---
api_host            |   API Host    |   https://<your company>.crowdstrike.com  |   String  |   True    |   CrowdStrike API Host URL.
client_id           |   Client ID   | N/A | Authentication  |   True    |   CrowdStrike API id for QRadar.
client_secret       |   Client Secret   |   N/A |   Authentication  |   True    |   CrowdStrike API secret for QRadar.
limit               |   Limit | 100 |   Integer |   False   |   Maximum number of alerts to return per poll.