# SCHJMS Connector
====================

OUT-SCHJMS Connector is responsible for provisioning school student information from IDM.WIN into ERN related systems.
This Connector will require to satisfy the following CRUD events:

    1.  ADD
    2.  MODIFY
    3.  DELETE
    4.  MOVE
The scope for this connector are active school student accounts : OU=SCH
The association key is the SRN number (detschstudentnumber). The unique identifier for the connector is schjms#

## Features

### Security

The connector is a queue to queue workflow. Access to the TIBCO JMS queues is protected by a username/password pair.
This connector will utilise the existing IDMiS TIBCO framework.
Password and Usernames are to be in line with the rest of IDMiS (stored in the idmis.properties file).

## Build

This project uses maven to build a WAR file for deployment to JBoss EAP6.

    mvn package

## Installation

Use your standard JBoss EAP6 deployment strategy for WAR files.

## Contribute

- [Issue Tracker](https://jirait.det.nsw.edu.au/browse/IDM-924)
- [Source Code](https://buildsystem.det.nsw.edu.au/stash/projects/IDMIS6/repos/out-schjms/browse)

## Support

For feature requests or advice on how to add a new backend data source or type,
please contact the Common Systems & Services team leads.

For runtime issues please raise an incident in Remedy and assign it to the *CSS
Support* group.
