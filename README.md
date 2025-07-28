# Network Management Portal

A React-based web application for managing and monitoring a network device.

## Features

*   **Dashboard:** View system uptime, CPU usage, memory usage, and disk usage.
*   **User Management:** View and manage DHCP leases.
*   **Firewall Management:** Block and unblock websites, view DNS logs.
*   **Active Connections:** View active network connections and interfaces.
*   **Network Traffic Viewer:** Monitor network traffic in real-time.
*   **ARP Table Management:** View and manage the ARP table.
*   **Settings:** Configure system settings like hostname and DNS servers.

## Installation

1.  Clone the repository:
    ```bash
    git clone https://github.com/your-username/network-management-portal.git
    ```
2.  Install the dependencies:
    ```bash
    npm install
    ```

## Usage

1.  Start the development server:
    ```bash
    npm start
    ```
2.  Open your browser and navigate to `http://localhost:3000`.
3.  Log in with the default credentials:
    *   **Username:** admin
    *   **Password:** admin

## Components

The application is built with the following React components:

*   `Login`: Handles user authentication.
*   `Dashboard`: Displays system status and usage charts.
*   `UserManagement`: Manages DHCP leases.
*   `FirewallManagement`: Manages firewall rules and DNS logs.
*   `ActiveConnections`: Displays active network connections.
*   `Settings`: Manages system settings.
*   `NetworkTrafficViewer`: Displays network traffic statistics.
*   `ARPTableManagement`: Manages the ARP table.
*   `TrafficMonitor`: Provides a live view of network traffic.

## API Endpoints

The application interacts with a network device's API at `https://192.168.1.1/api/v2`. The following endpoints are used:

*   `/status/system`: Get system status and uptime.
*   `/status/dhcp_server/leases`: Get DHCP leases.
*   `/services/dns_resolver/domain_overrides`: Get and manage domain overrides.
*   `/status/logs/firewall`: Get firewall logs.
*   `/status/interfaces`: Get network interface status.
*   `/system/hostname`: Get and set the system hostname.
*   `/system/dns`: Get and set DNS server settings.
*   `/diagnostics/halt_system`: Shut down the system.
*   `/diagnostics/reboot`: Reboot the system.
*   `/diagnostics/arp_table`: Get the ARP table.
*   `/diagnostics/command_prompt`: Execute shell commands.
