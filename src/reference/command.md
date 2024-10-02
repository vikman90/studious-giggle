# Command Call

## Configuration Files

- **ossec.conf**: The main configuration file for the Wazuh Agent. It defines the agent’s behavior, including monitored paths, server connections, and active response rules.

  Example configuration block:
  ```xml
  <agent>
    <server>
      <address>192.168.1.100</address>
      <port>1514</port>
      <protocol>udp</protocol>
    </server>
    <notify_time>10</notify_time>
    <disable_reconnect>no</disable_reconnect>
  </agent>
  ```

- **agent.conf**: The agent-specific configuration for customizing behavior per agent installation.

## Commands

- **agent-control**: A command-line utility to control and manage the Wazuh Agent.

  Common commands:
  ```bash
  /var/ossec/bin/agent-control -s    # Show agent status
  /var/ossec/bin/agent-control -r    # Restart the agent
  ```

## Logging

Wazuh Agent logs all its operations in the following files:

- **ossec.log**: Primary log file located in `/var/ossec/logs/ossec.log` on Linux/macOS or `C:\Program Files (x86)\ossec-agent\logs\ossec.log` on Windows.

  Example log entries:
  ```
  2024/09/30 12:30:45 ossec-agent: INFO: Agent started successfully.
  2024/09/30 12:35:10 ossec-agent: WARNING: Connection to the manager failed.
  ```

## Useful Links

- [Wazuh Documentation](https://documentation.wazuh.com/current/)
- [Wazuh GitHub Repository](https://github.com/wazuh/wazuh)
