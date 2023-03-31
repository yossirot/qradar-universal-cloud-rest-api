# CyberInt Parameters Configuration
Parameter                           | Name | Default Value | Type | Required (True/False) | Description
---                                 | --- | --- | --- |--- |---
hostname                            | Host Name | https://<instance name>.cyberint.io | String | True | IP or URL for the instance.
api_key                             | API Key | False | Authentication | True | Cyberint API key for QRadar.
severity                            | Severity | "very_high" "high", "medium", "low" | Array of String | False | You can specify the alert severity to pull.
status                              | Status | "open", "acknowledged", "closed" | Array of String | False | You can specify the alert status to pull.