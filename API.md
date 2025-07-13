# Zabbix API

The Zabbix API allows you to programmatically retrieve and modify the configuration of Zabbix and provides access to historical data. It is widely used to:

*   Create new applications to work with Zabbix.
*   Integrate Zabbix with third party software.
*   Automate routine tasks.

## Getting Started

The Zabbix API is a web-based API that uses the JSON-RPC 2.0 protocol. You can access the API by sending HTTP POST requests to the `api_jsonrpc.php` file in your Zabbix installation.

To learn more about the Zabbix API, please refer to the [official documentation](https://www.zabbix.com/documentation/current/en/manual/api).

## Authentication

To use the Zabbix API, you need to authenticate with a user who has API access. You can authenticate by using the `user.login` method.

## Example

The following is an example of how to use the Zabbix API to retrieve the list of hosts:

```json
{
    "jsonrpc": "2.0",
    "method": "host.get",
    "params": {
        "output": "extend"
    },
    "auth": "038e1d7b1735c6a5436ee9eae095879e",
    "id": 1
}
```

This request will return a list of all the hosts in your Zabbix installation.

## API Reference

For a complete list of all the available methods and their parameters, please refer to the [API reference](https://www.zabbix.com/documentation/current/en/manual/api/reference).
