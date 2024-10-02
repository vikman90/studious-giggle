# Agent Configuration

This document outlines the configurable options available in the `etc/wazuh-agent/agent.yml` file for the Wazuh Agent. The configuration is divided into different sections, each containing relevant options to customize the agent’s behavior.

## Agent

| Option   | Description                 | Default value |
|----------|-----------------------------|---------------|
| server   | The address of the Wazuh server to connect to. | None          |
| timeout  | Connection timeout, specified in seconds. | 1s            |

## Inventory

| Option   | Description                                       | Default value |
|----------|---------------------------------------------------|---------------|
| interval | The frequency of the inventory scan (e.g., 1d for daily). | 1d            |
| hardware | Whether to scan the hardware components of the system.     | yes           |
| os       | Whether to scan the operating system information.          | yes           |
| network  | Whether to scan network configuration and details.         | yes           |
| packages | Whether to scan installed software packages.               | yes           |
| ports    | Whether to scan open ports on the system.                  | yes           |
