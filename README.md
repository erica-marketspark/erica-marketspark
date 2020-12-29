# Cradlepoint

We will be carrying Cradlepoint equipment in the near short-term and have researched options on how to integrate CradlePoint with CMDC-API to get status.

## Cradlepoint Docs

> Cradlepoint NetCloud Manager (NCM) is an SaaS-type server that enables the remote management of network devices, including routers and access points. This specification describes a RESTful API that can be used by web applications to access the service.

- [Documentation](https://developer.cradlepoint.com/documentation)

## Netcloud Manager (NCM) API 2.0 Overview

- [Getting Started](https://developer.cradlepoint.com/)
- [Instructions](https://customer.cradlepoint.com/s/article/NCM-APIv2-Overview): ECM key values in Dev Team 1Password: “READ ONLY - NetCloud API - ECM Keys”

## Status Change Notification/Integration

Webhooks/Push notification abilities have not been provided by the Cradlepoint NCM API.

**Alternatives:**

- [Email Alerts](https://www.cradlepointecm.com/ecm.html#logs/alert_log) can be configured through the Cradlepoint Enterprise Cloud Manager (ECM) UI with optional method to parse email using [Sendgrid](https://sendgrid.com/docs/API_Reference/Parse_Webhook/inbound_email.html)

  - [Docs](https://customer.cradlepoint.com/s/article/Alerting-and-Reporting-with-NCM)
  - [Cradlepoint ECM UI](https://www.cradlepointecm.com/ecm.html#devices/routers): Login using “Cradlepointecm” password in Dev Team 1Password

- Monitoring by polling the routers endpoint for all router state (online/offline/initialized)
  changes on your account.

  - [API sample](https://github.com/cradlepoint/api-samples/blob/master/monitoring/samples/router_online_offline.py)

- Configure Routers Directly using Cradlepoint's Netcloud OS (NCOS SDK) to send push notifications

  > Cradlepoint’s NetCloud OS (NCOS) SDK provides the ability to customize the functionality of Cradlepoint devices with applications written in Python. Python applications written with the SDK are securely downloaded to the device and enabled using NetCloud Manager (NCM). Cradlepoint’s SDK allows for extending and enhancing the functionality of Cradlepoint devices, FOG computing, and managing IoT devices.

  - [Docs](https://customer.cradlepoint.com/s/article/NCOS-SDK-v3)
  - [Example Code](https://github.com/cradlepoint/sdk-samples/blob/master/app_template_csclient/csclient.py)
