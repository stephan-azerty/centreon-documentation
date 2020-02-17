# Easy Vista Open ticket connector

## Table of contents
1. [How it works](#how-it-works)
2. [Compatibility](#compatibility)
3. [Requirements](#requirements)
4. [Possibilities](#possibilities)

## How it works <a name="how-it-works"></a>
Easy Vista open-tickets provider uses the Easy Vista SOAP API to open incidents about your monitoring alerts.

![architecture](img/ot-easyvista-architecture.png)

## Compatibility <a name="compatibility"></a>
This integration is (at least) compatible with the following Easy Vista versions:

**To be determined**

## Requirements
Before going any further, make sure that you correctly setup [centreon-open-ticket](https://documentation.centreon.com/docs/centreon-open-tickets/en/latest/installation/index.html)
into your Centreon instance

Our provider requires the following parameters:

| Parameter | Example of value |
| --------- | ---------------- |
| Address | 192.168.0.27 |
| Webservice Path | /WebService/SmoBridge.php |
| Username | centreon |
| Password | MyPassword |
| Timeout | 60 |

## Possibilities <a name="possibilities"></a>
As of now, the provider is able to open a ticket with the following parameters

- Requestor
- Urgency
- Severity
- Asset
- External reference
- Phone
- Recipient
- Origin
- CI