---
title: Rituals Perfume Genie
description: "Instructions on how to set up Rituals Perfume Genie within Home Assistant."
logo: rituals.svg
ha_category:
  - Fan
ha_release: 0.101
ha_iot_class: Cloud Polling
---

The `rituals` platform allows one to control the [Rituals Perfume Genie](https://www.rituals.com/en-us/perfume-genie.html) smart air freshener. Before using this integration, you will need to follow the instructions in the official Rituals Perfume Genie app ([Android](https://play.google.com/store/apps/details?id=com.rituals.diffuser2) or [iOS](https://apps.apple.com/us/app/perfume-genie/id1259103949)) in order to create a Rituals account and connect the desired device(s).

## Configuration

To enable this integration, add the following lines to your `configuration.yaml`:

```yaml
switch:
  - platform: rituals
    email: RITUALS_EMAIL
    password: RITUALS_PASSWORD
```

{% configuration %}
username:
  description: Email address used for your Rituals account
  required: true
  type: string
password:
  description: Password used for your Rituals account
  required: true
  type: string
{% endconfiguration %}