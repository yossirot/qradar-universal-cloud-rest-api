# Rapid7 ThreatCommand Parameters Configuration
Parameter                           | Name | Default Value | Type | Required (True/False) | Description
---                                 | --- | --- | --- |--- |---
hostname                            | Host Name | https://api.ti.insight.rapid7.com | String | True | URL for the instance.
account_id                          | Account ID | False | Authentication | True | Threat Command account ID.
api_key                             | API Key | False | Authentication | True | Threat Command API key for QRadar.
severity                            | Severity | "High", "Medium", "Low" | String | False | you can specify the alert severity to pull.
is_closed                           | Is Closed | True | Bool | False | Change to folse for ignoring closed alerts.

# How to Generate API token
1. Log on to your Rapid7 Threat Command instance through: https://api.ti.insight.rapid7.com.

2. At the left side of the screen press the SETTINGS button and then enter the "Subscription".

3. In the Downloads section in the right side press at "Generate API key".

4. Here you can see your account id and your api key.

# QRadar Log Source Configuration
If you want to ingest data from an endpoint using Universal Rest API Protocol, configure a log source on the QRadar® Console using the Workflow field so that the defined endpoint can communicate with QRadar by using the Universal Rest API protocol.

1. Log in to QRadar.

2. Click the Admin tab.

3. To create DSM, click the DSM editor app icon.

4. Then click Create New and name it "Cyberint API".

4. To create the log source, click the QRadar Log Source Management app icon.

5. Click New Log Source > Single Log Source.

6. On the Select a Log Source Type page, Select a Log Source Type Cyberint API and click Select Protocol Type (Universal Rest API).

7. On the Select a Protocol Type page, select a protocol and click Configure Log Source Parameters.

8. On the Configure the Log Source parameters page, configure the log source parameters and click Configure Protocol Parameters.

9. On the Configure the Protocol Parameters page, configure the protocol-specific parameters (Workflow and Workflow Parameter Values).

10. In the Test protocol parameters window, click Start Test.

10. To fix any errors, click Configure Protocol Parameters. Configure the parameters and click Test Protocol Parameters.

11. Click Finish
