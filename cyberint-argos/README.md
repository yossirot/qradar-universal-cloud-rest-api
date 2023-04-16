# CyberInt Parameters Configuration
Parameter                           | Name | Default Value | Type | Required (True/False) | Description
---                                 | --- | --- | --- |--- |---
hostname                            | Host Name | https://\<MyCompuny>.cyberint.io | String | True | URL of your Cyberint instance.
api_key                             | API Key | False | Authentication | True | Cyberint API token for QRadar.
severity                            | Severity | "very_high" "high", "medium", "low" | Array of String | False | You can specify the alert severity to pull.
status                              | Status | "open", "acknowledged", "closed" | Array of String | False | You can specify the alert status to pull.

# How to Generate API token
1. Log on to your Cyberint instance through: https://\<MyCompuny>/cyberint.io.

2. At the top right of the screen press the profile button and then enter the "USER SETTINGS".

3. In the user settings press at three doted in the top right.

4. Press the "Generate API Token" button.

5. Here you can see your api token.

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
