---
id: isilog
title: Isilog
---

## How it works

Isilog open-tickets provider uses the Isilog SOAP API to open incidents about
your monitoring alerts.

![architecture](../../assets/integrations/open-tickets/ot-isilog-architecture.png)

## Compatibility

This integration is (at least) compatible with the following Isilog versions:

**to be determined**

## Requirements

Before going any further, make sure that you correctly setup
[centreon-open-ticket](https://documentation.centreon.com/docs/centreon-open-tickets/en/latest/installation/index.html)
into your Centreon instance

Our provider requires the following parameters:

| Parameter | Example of value                                |
| --------- | ----------------------------------------------- |
| Address   | demo.iws-saas.fr/isilogwebsystem                |
| Username  | DEMO                                            |
| Password  | MyPassword                                      |
| Database Name | MYITSM                                      |
| Protocol  | https                                           |
| Timeout   | 60                                              |

## Possibilities

As of now, the provider is able to retrieve the following objects from Isilog:

  - Categories
  - Services
  - Impacts
  - Urgencies
  - Qualifiers
  - Origins
  - Teams
  - Users
  - Business Units (BU)
  - Sites
  - Customers

## Isilog Configuration

To retrieve all those informations you need to configure Isilog webservices and put their names in the provider configuration.

### Categories webservice

![categories webservice](../../assets/integrations/open-tickets/ot-isilog/ot-isilog-webservice-categories.gif)

### Sites webservice

![sites webservice](../../assets/integrations/open-tickets/ot-isilog/ot-isilog-webservice-sites.gif)

### Business Units webservice

![BU webservice](../../assets/integrations/open-tickets/ot-isilog/ot-isilog-webservice-bu.gif)

### Teams webservice

![teams webservice](../../assets/integrations/open-tickets/ot-isilog/ot-isilog-webservice-teams.gif)

### Users webservice

![users webservice](../../assets/integrations/open-tickets/ot-isilog/ot-isilog-webservice-users.gif)

### Impacts webservice

![impacts webservice](../../assets/integrations/open-tickets/ot-isilog/ot-isilog-webservice-impacts.gif)

### Urgencies webservice

![urgencies webservice](../../assets/integrations/open-tickets/ot-isilog/ot-isilog-webservice-urgencies.gif)

### Services webservice

![services webservice](../../assets/integrations/open-tickets/ot-isilog/ot-isilog-webservice-services.gif)

### Others webservice

![others webservice](../../assets/integrations/open-tickets/ot-isilog/ot-isilog-webservice-others.gif)

## Centreon configuration

When your desired webservices are configured, you can just put their name in your provider configuration and test your connection

![test webservice](../../assets/integrations/open-tickets/ot-isilog/ot-isilog-webservice-test.png)
