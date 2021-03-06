---
title: "Thomson"
description: "Instructions on how to integrate Thomson routers into Home Assistant."
logo: technicolor.png
ha_category:
  - Presence Detection
ha_release: 0.7
redirect_from:
 - /components/device_tracker.thomson/
---


Thomson produced networking equipment (under the brand name SpeedTouch) till 2010 and was then renamed to Technicolor.

This platform allows you to detect presence by looking at connected devices to a [Thomson](http://www.technicolor.com) device.

To use this device tracker in your installation, add the following to your `configuration.yaml` file:

```yaml
# Example configuration.yaml entry
device_tracker:
  - platform: thomson
    host: YOUR_ROUTER_IP
    username: YOUR_ADMIN_USERNAME
    password: YOUR_ADMIN_PASSWORD
```

{% configuration %}
host:
  description: The IP address of your router, e.g., 192.168.1.1.
  required: true
  type: string
username:
  description: The username of an user with administrative privileges, usually *admin*.
  required: true
  type: string
password:
  description: The password for your given admin account.
  required: true
  type: string
{% endconfiguration %}

See the [device tracker integration page](/components/device_tracker/) for instructions how to configure the people to be tracked.
