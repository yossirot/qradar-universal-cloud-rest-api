# QRadar Universal Cloud Rest API

<h1 align="center">
  <img width="auto" height="50px" src="https://awsmp-logos.s3.amazonaws.com/28ee383e-9c31-4664-a692-a00a472feb1c/08243c42094d411568f25ffd5ae3e1e9.png"/>
  <img width="auto" height="50px" src="https://assets.extrahop.com/images/logos/ibm-qradar.png"/>
</h1>


## IBM QRadar Universal Cloud Connector
The QRadar Universal Cloud Rest API is a powerful feature that can help security teams enhance their visibility by easily gathering data from a wide range of REST API cloud-based applications and services. With the Universal Cloud REST API Protocol, users can create log sources for REST API compatible data sources that are currently not supported by IBM. This means that organizations can quickly and easily connect to cloud-based or on-premise endpoints that were previously inaccessible.

The Universal Cloud REST API Protocol also includes pre-configured workflows for select data sources, which can substantially reduce the time required to create new log sources. Furthermore, users can tailor the data to their specific use cases by defining normalized properties, classifying event data, and extracting custom event properties using the DSM Editor. By connecting their data sources with the Universal Cloud REST API Protocol, organizations can augment their threat detection abilities, and analysts can easily access key investigation information in their workspace using QRadar's Analyst Workflow, minimizing the need to navigate elsewhere for additional context. Overall, the QRadar Universal Cloud Rest API is a powerful tool that can help organizations adapt to the ever-changing digital landscape and improve their security posture.


## Supported version
[![7.3.2 QRadar](https://img.shields.io/badge/QRadar-%20v7.3.2-yellow.svg)](https://opensource.org/licenses/)
[![7.3.2 QRadar](https://img.shields.io/badge/QRadar_Universal_Cloud_REST_API-%20v2-yellow.svg)](https://opensource.org/licenses/)


## Terminology
As you configure the Universal Cloud REST API, familiarize yourself with the following terms:

Workflow: An XML document that outlines the event retrieval process. It defines one or more parameters, which can have assigned values within the XML or derive values from the Workflow Parameter Values XML document. The Workflow comprises several actions that run sequentially. When the Workflow is initiated, the parameter values are included in the State. As the Workflow runs, actions can access and modify the State.

Workflow Parameter Values: The input parameters for a Workflow instance, stored in an XML file. These values are a set of key/value pairs, and each key must match a parameter defined in the corresponding Workflow.

## Authors
At QMasters, we believe in giving back to the community and our customers. As a team that has worked extensively with SIEMs since the start of our journey, we understand the importance of data in effective threat detection and response. We work closely with our customers and vendors to provide them with the tools they need to make the most of their security data. By developing and sharing tools like the QRadar Universal Cloud Rest API, we aim to contribute to the wider security community and help organizations improve their security posture.
## Useful Links

 - [IBM GitHub](https://github.com/IBM/IBM-QRadar-Universal-Cloud-REST-API)
 - [Universal Cloud REST API protocol](https://www.ibm.com/docs/en/qsip/7.4?topic=configuration-universal-cloud-rest-api-protocol)


## Support
To request support or suggest the development of new features for the QRadar Universal Cloud Rest API, please contact our support team at support@qmasters.co.