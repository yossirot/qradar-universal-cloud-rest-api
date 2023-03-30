# Fortress Parameters Configuration
Parameter                           | Name | Default Value | Type | Required (True/False) | Description
---                                 | --- | --- | --- |--- |---
api_host                            | API Host | https://develop-api.qfortress.ai | String | True | IP or URL for the instance.
api_key                             | API Key | False | Authentication | True | 
api_secret                          | API Secret | False | Authentication | True | 
severity                            | Severity | "CRITICAL","HIGH","MEDIUM","LOW","NONE" | array of strings | False | his parameter is an array of strings used to filter alerts by severity.
status                              | Status | "OPEN","CLOSED","DISMISSED","QUARANTINED" | array of string | False | his parameter is an array of strings used to filter alerts by status.
service_type                        | Service Type | "EDP","WEB","MAIL","CLOUD_STORAGE","VMDR","ATTACK_SIMULATOR","MERLIN_AI","SANDBOX" | array of string | False | this parameter is an array of strings used to filter alerts by service type.
page_size                           | page Size | 100 | integer | True | 
time_zone                           | Time Zone | UTC | Authentication | string | 
