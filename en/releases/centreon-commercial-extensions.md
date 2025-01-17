---
id: centreon-commercial-extensions
title: Commercial Extensions
---

## Introduction

You can find in this chapter all changelogs concerning **Centreon Commercial
Extension**.

> It is very important when you update your system to refer to this section in
> order to learn about behavior changes or major changes that have been made on
> this version. This will let you know the impact of the installation of these
> versions on the features you use or the specific developments that you have
> built on your platform (modules, widgets, plugins).

If you have feature requests or want to report a bug, please contact support.

## Centreon MAP release notes

### 20.10.2

* [Enhancement] Full TLS compliance has been added for communication with Broker component
* [Fix] Upgrading from previous versions could cause a failed restart of centreon-map service
* [Fix] Fresh install or upgrade could result in wrong permissions for centreon-map media folder
* [Fix] Adding or deleting a Downtime from the Web-UI could result in loss of connection with Broker
* [Fix] Creating a map with empty name could cause a failure to load the Monitoring>Map menu
* [Fix] Adding an Output in Studio could sometimes result in mis formatted metric
* [Fix] WhatsUp events were unnecessarily raised in web sessions potentially causing performance issues
* [Fix][API] Requesting token from Swagger-ui could result in an error

### 20.10.1

* Saving Geo Views on a Custom View Map widget was impossible due to missing "Save" button
* Sharing usage statistics metrics between MAP server and Central through HTTPS failed
* Creating Links through REST API can now make use of 'bendpoints', 'displayValue' and 'displayPercent' properties
* Adding Centreon resources when creating an Output widget through REST API is now possible
* Installing a fresh MAP Studio resulted in automated back-up failure

### 20.10.0

#### Enhancements

-   The license is now entirely managed on the Centreon Central server.

#### Faster server for complex maps

This version lays the foundations for the evolution of the experience
in creating and visualizing maps.

The first step being the birth of a new Centreon MAP server (code name
**"NG"** for "New Generation"), which has been designed to be more
powerful, faster and lighter.

The server is in **experimental phase** and is subject to evolution.

It is currently only used for visualizing maps. Maps creation and edition
still use the server as we know it.

As for the Centreon interface, everything has been done to be able to
use these two servers. It is then possible to switch the consultation of
maps from one server to the other easily.

To use it, it is necessary to install and activate it. Refer to the
[dedicated documentation](../graph-views/install.html#centreon-map-ng)

## Centreon BAM release notes

### 20.10.0

- [Configuration] Update style of pages *Business Activities* and
  *Business Views*

## Centreon MBI release notes

### 20.10.0

- Compatibility with Centreon 20.10

## Centreon Auto Discovery release notes

### 20.10.2

#### Bugfixes

- [Host Discovery] Long values in *host.ip* field cause "Error when sorting
  and filtering host modification results" issue
- [Host Discovery] Save script now runs on CentOS 8

#### Enhancements

- [Host Discovery] Add a confirmation dialog when deleting a job
- [Host Discovery] Change wording "Additional parameters" to "Discovery
  parameters"

### 20.10.1

#### Bugfixes

- Double upgrade scripts in previous build lead to sql error in log

### 20.10.0

> Refer to the [Gorgone module configuration](../monitoring/discovery/administration.html#gorgone-module-configuration)
> to make sure the configuration matches minimal prerequisites.

> If a discovery is performed on a Remote Server or a Poller, make sure
> the server is using the latest 20.10 components.

> On a Remote Server, the Autodiscovery module can be uninstalled through
> the `Administration > Extensions > Manager` menu so it will not raise
> useless errors in Gorgone's log.

#### Host Discovery

Host Discovery wizard now allows to schedule your discoveries using several
fashion: yearly, monthly, daily, hourly and even every x minutes.

Scheduled discovery jobs can be paused and resumed at any time.

Discovery result can also be automatically processed to add, disable and
when necessary re-enable the hosts in the configuration.

If you decide to manually add the hosts from the job's result page, the
mapping rule can now be edited and saved from this page to match
your needs by applying the rule directly on the result.

The new *exclusion* and *inclusion* mappers will help you decide which hosts
are meant to be added in the configuration, and the ones that should be
disabled or enabled.

Take a look at this example to fully understand their impacts:
[Dynamically update your configuration](../monitoring/discovery/hosts-discovery.html#dynamically-update-your-configuration)

#### Service Discovery

Service Discovery is now using Gorgone to execute the discovery plugins,
and therefore it uses Gorgone's communication system and not anymore
standalone SSH connections.

#### Bugfixes

- Contains all fixes up to version 20.04.6

## Centreon Plugin Packs Manager release notes

### 20.10.0

- Compatibility with Centreon 20.10

## Centreon License Manager release notes

### 20.10.1

#### Bug fixes

- After adding a license or a token the user must access to associated functionalities
- Rights issues with the gnupg library with multiple users (only with Docker)
- Disable 'Add' button when input is empty

### 20.10.0

- Compatibility with Centreon 20.10

## Centreon Anomaly Detection

### 20.10.0

- Compatibility with Centreon 20.10
