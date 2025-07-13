# Zabbix

![Zabbix logo](misc/images/docs/zabbix_logo.svg?raw=true)

Zabbix is an enterprise-class, open-source distributed monitoring solution that’s designed to monitor the performance and availability of network devices, servers, services, and other IT resources.

## Project Overview

Zabbix is a flexible solution that can monitor anything from a simple, standalone application to a large-scale environment, with features including:

*   **Resource discovery:** Discover network entities, server resources, and onboard/offboard devices. Use out-of-the-box integrations (templates) to monitor anything form a low-level device to a SAAS service.
*   **Metric acquisition:** Use an agent or agent-less approach for metric acquisition from any source – devices, sensors, operating systems, virtualization platforms, container platforms like Docker, Kubernetes, cloud infrastructures, databases, webpages, Java ecosystems, application servers, API endpoints, business applications, and many more.
*   **Root cause analysis and problem detection:** Count on high-performance, real-time problem detection that correlates both existing and incoming problems and performs root cause analyses.
*   **Incidents, alerts, and notifications:** Receive an alert when an issue is triggered (proactively or post-mortem) in the ecosystem. Use multiple messaging channels (including Slack, JIRA, Microsoft Teams, email or text messages) to get notified about the different types of events occurring in your environment.
*   **“Single pane of glass” overview:** Visualize collected data and monitoring events in graphs, lists, geomaps, and network topology maps.
*   **Multitenancy and distributed monitoring:** Enjoy the convenience of one monitoring solution for multiple data centers, departments, and organizations, and monitor remote locations behind firewalls with remote command execution capability.
*   **Unparalleled flexibility:** Adapt Zabbix to your needs and utilize built-in functionalities, including the ability to stream metrics and events over HTTP, reporting, auditing, security, service SLA calculations, and many more.

## Getting Started

### Prerequisites

*   A web server (Apache, Nginx, or IIS)
*   A database (MySQL, PostgreSQL, or Oracle)
*   PHP 7.2 or later

### Installation

1.  Download the latest version of Zabbix from the [official website](https://www.zabbix.com/download).
2.  Follow the [installation manual](https://www.zabbix.com/documentation/current/en/manual/installation) to install Zabbix on your server.

### Quick Start

Once Zabbix is installed, you can start monitoring your resources by following these steps:

1.  Log in to the Zabbix UI.
2.  Create a new host and link it to a template.
3.  Install the Zabbix agent on the host.
4.  Start the Zabbix agent.

For more detailed instructions, please refer to the [Zabbix documentation](https://www.zabbix.com/documentation/current/en/).

## Project Structure

The Zabbix codebase is organized into the following directories:

*   `src`: The source code for the Zabbix server, agent, and other components.
    *   `zabbix_server`: The C-based Zabbix server.
    *   `zabbix_agent`: The C-based Zabbix agent.
    *   `go`: The Go-based Zabbix agent.
*   `ui`: The PHP-based Zabbix web interface.
*   `database`: The SQL schemas and data for various databases.
*   `templates`: A large collection of monitoring templates in YAML format.

## Contribution Guidelines

We welcome contributions to Zabbix! If you would like to contribute, please follow these steps:

1.  Fork the Zabbix repository on GitHub.
2.  Create a new branch for your changes.
3.  Make your changes and commit them to your branch.
4.  Submit a pull request to the Zabbix repository.

Please make sure to follow the Zabbix coding standards and to include tests for your changes.

## License

Zabbix is distributed under the [AGPL-3.0-only](COPYING) license.
