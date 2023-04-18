# Fortress Parameters Configuration
Parameter                           | Name | Default Value | Type | Required (True/False) | Description
---                                 | --- | --- | --- |--- |---
api_host                            | API Host | https://develop-api.qfortress.ai | String | True | URL for the instance.
api_key                             | API Key | False | Authentication | True | Fortress API key for QRadar
api_secret                          | API Secret | False | Authentication | True | Fortress API secret for QRadar
severity                            | Severity | "CRITICAL", "HIGH", "MEDIUM", "LOW", "NONE" | array of strings | False | this parameter is an array of strings used to filter alerts by severity.
status                              | Status | "OPEN", "CLOSED", "DISMISSED", "QUARANTINED" | array of strings | False | this parameter is an array of strings used to filter alerts by status.
service_type                        | Service Type | "EDP", "MAIL", "CLOUD_STORAGE", "VMDR" | array of strings | False | this parameter is an array of strings used to filter alerts by service type.
page_size                           | page Size | 100 | integer | false | Max number of alerts to return per poll
time_zone                           | Time Zone | UTC | string | false | Select your time zone

# How to Generate API token
1. Log on to your Fortress instance through: https://develop-api.qfortress.ai.

2. At the left side of the screen press the settings button and then enter the "Admin Configuration".

3. In the Admin Configuration press at API Management.

4. Press the "+Add API key" button.

5. Insert the API name and choose the "View Alerts" permission, and press "Add".

5. Here you can see your api token.

# QRadar Log Source Configuration
If you want to ingest data from an endpoint using Universal Rest API Protocol, configure a log source on the QRadar® Console using the Workflow field so that the defined endpoint can communicate with QRadar by using the Universal Rest API protocol.

1. Log in to QRadar.

2. Click the Admin tab.

3. To create DSM, click the DSM editor app icon.

4. Then click Create New and name it "Fortress API".

4. To create the log source, click the QRadar Log Source Management app icon.

5. Click New Log Source > Single Log Source.

6. On the Select a Log Source Type page, Select a Log Source Type Fortress API and click Select Protocol Type (Universal Rest API).

7. On the Select a Protocol Type page, select a protocol and click Configure Log Source Parameters.

8. On the Configure the Log Source parameters page, configure the log source parameters and click Configure Protocol Parameters.

9. On the Configure the Protocol Parameters page, configure the protocol-specific parameters (Workflow and Workflow Parameter Values).

10. In the Test protocol parameters window, click Start Test.

10. To fix any errors, click Configure Protocol Parameters. Configure the parameters and click Test Protocol Parameters.

11. Click Finish
