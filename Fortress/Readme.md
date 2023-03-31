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
