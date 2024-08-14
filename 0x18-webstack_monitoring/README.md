# 0x18. Webstack Monitoring

## Concepts
For this project, you should understand these concepts:
- Monitoring
- Server

## Background Context
“You cannot fix or improve what you cannot measure” is a famous saying in the tech industry. In the age of data-ism, monitoring how our software systems are performing is crucial. This project focuses on implementing one of many tools to measure what is happening on our servers.

Web stack monitoring can be broken down into two categories:
1. **Application monitoring**: Gathering data about your running software to ensure it is behaving as expected.
2. **Server monitoring**: Gathering data about your virtual or physical server to ensure they are not overloaded (e.g., CPU, memory, disk, or network overload).

## Tasks

### 0. Sign up for Datadog and install `datadog-agent`
**Mandatory**

For this task, sign up for a free Datadog account at [Datadog](https://www.datadoghq.com/). Once signed up, follow the instructions on the website to install the Datadog agent.

- Sign up for Datadog using the US website (`https://app.datadoghq.com`).
- Use the US1 region.
- Install `datadog-agent` on `web-01`.
- Create an application key.
- Copy-paste your Datadog API key and application key into your Intranet user profile.
- Your server `web-01` should be visible in Datadog under the hostname `XX-web-01`.

You can validate it using this [API](https://docs.datadoghq.com/api/latest/).

If needed, update the hostname of your server.

**Repository:**
- GitHub repository: `alx-system_engineering-devops`
- Directory: `0x18-webstack_monitoring`

### 1. Monitor some metrics
**Mandatory**

Datadog can report a wide range of system metrics. Set up some monitors within the Datadog dashboard to monitor and alert you of key metrics.

- Set up a monitor that checks the number of read requests issued to the device per second.
- Set up a monitor that checks the number of write requests issued to the device per second.

**Repository:**
- GitHub repository: `alx-system_engineering-devops`
- Directory: `0x18-webstack_monitoring`

### 2. Create a dashboard
**Mandatory**

Create a dashboard with different metrics displayed to get a few visualizations.

- Create a new dashboard.
- Add at least 4 widgets to your dashboard (any type, monitoring whatever you'd like).
- Create the answer file `2-setup_datadog`, which contains the `dashboard_id` on the first line. You may need to use Datadog's API to retrieve the dashboard ID.

**Repository:**
- GitHub repository: `alx-system_engineering-devops`
- Directory: `0x18-webstack_monitoring`
- File: `2-setup_datadog`
