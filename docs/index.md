---
title: MailHog Lando Plugin
description: Add a highly configurable mailhog service to Lando for local development with all the power of Docker and Docker Compose.
next: ./config.html
---

# MailHog

[MailHog](https://github.com/mailhog/MailHog) is an email testing tool for developers.

You can easily add it to your Lando app by adding an entry to the [services](https://docs.lando.dev/core/v3/lando-service.html) top-level config in your [Landofile](https://docs.lando.dev/core/v3).

```yaml
services:
  myservice:
    type: mailhog
```

## Supported versions

*   **[v1.0.1](https://hub.docker.com/r/mailhog/mailhog/)** **(default)**
*   [v1.0.0](https://hub.docker.com/r/mailhog/mailhog/)
*   [custom](https://docs.lando.dev/core/v3/lando-service.html#overrides)

## Patch versions

This service does not support patch versions but if you **really** need something like that you could consider using either a [custom compose service](https://docs.lando.dev/plugins/compose) or a service [overrides](https://docs.lando.dev/core/v3/lando-service.html#overrides).

