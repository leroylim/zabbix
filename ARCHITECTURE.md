# Zabbix Architecture

This document provides a high-level overview of the Zabbix architecture.

## Components

The Zabbix architecture consists of the following major components:

*   **Zabbix Server:** The core of the Zabbix monitoring solution. It's responsible for collecting and storing data, detecting problems, and sending notifications.
*   **Zabbix Agent:** A lightweight agent that runs on the monitored hosts. It's responsible for collecting data from the host and sending it to the Zabbix server.
*   **Zabbix UI:** A web-based interface that allows you to view and manage your monitoring data.
*   **Database:** A database that stores all of the Zabbix monitoring data.

## Data Flow

The following diagram illustrates the data flow between the different components of the Zabbix architecture:

```
+----------------+      +----------------+      +----------------+
|  Zabbix Agent  |----->|  Zabbix Server |----->|    Database    |
+----------------+      +----------------+      +----------------+
                             ^
                             |
                             |
                             v
+----------------+      +----------------+
|   Zabbix UI    |<-----|  Zabbix Server |
+----------------+      +----------------+
```

1.  The Zabbix agent collects data from the monitored host and sends it to the Zabbix server.
2.  The Zabbix server stores the data in the database.
3.  The Zabbix UI queries the Zabbix server to display the monitoring data.

## Zabbix Server

The Zabbix server is a multi-process application that consists of the following major components:

*   **Pollers:** Responsible for collecting data from the monitored hosts.
*   **Trappers:** Responsible for receiving data from the Zabbix agents.
*   **Housekeeper:** Responsible for deleting old data from the database.
*   **Escalator:** Responsible for sending notifications.
*   **Configuration Syncer:** Responsible for keeping the configuration of the Zabbix server and agents in sync.

## Zabbix Agent

The Zabbix agent is a lightweight agent that can run in both passive and active modes.

*   **Passive Mode:** The agent listens for requests from the Zabbix server and sends back the requested data.
*   **Active Mode:** The agent proactively sends data to the Zabbix server.

The agent can be extended with user parameters, which are custom checks that can be used to monitor any type of data.

## Zabbix UI

The Zabbix UI is a web-based interface that allows you to view and manage your monitoring data. It's written in PHP and uses a custom MVC-like framework.

The UI provides a wide range of features, including:

*   Dashboards
*   Graphs
*   Maps
*   Reports
*   Configuration management
*   User management
