# Cradlepoint

We will be carrying Cradlepoint equipment in the near short-term and have researched options on how to integrate CradlePoint with CMDC-API to get status.

## Cradlepoint Docs

> Cradlepoint NetCloud Manager (NCM) is an SaaS-type server that enables the remote management of network devices, including routers and access points. This specification describes a RESTful API that can be used by web applications to access the service.

- [Documentation](https://developer.cradlepoint.com/documentation)

## Netcloud Manager (NCM) API 2.0 Overview

- [Getting Started](https://developer.cradlepoint.com/)
- [Instructions](https://customer.cradlepoint.com/s/article/NCM-APIv2-Overview): ECM key values in Dev Team 1Password: “READ ONLY - NetCloud API - ECM Keys”

## Status Change Notification/Integration

Webhooks/Push notification abilities have not been provided by the NCM API.

**Alternatives:**

- Email Alerts: (https://customer.cradlepoint.com/s/article/Alerting-and-Reporting-with-NCM#alert-defs)
- API sample shows examples for monitoring using polling: (https://github.com/cradlepoint/api-samples/blob/master/monitoring/samples/router_online_offline.py)
-
