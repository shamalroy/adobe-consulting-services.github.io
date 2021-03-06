---
layout: acs-aem-commons_feature
title: Syslog Integration
description: Send log messages to remote systems
date: 2014-01-10
thumbnail: /images/syslog/thumbnail.png
tags: acs-aem-commons-features
categories: acs-aem-commons features
initial-release: 1.5.0
---

# Purpose

Using this OSGi configured Logback appender, you can easily send log messages to a syslog server, either one internally hosted or hosted on a SaaS syslog service.

# How to Use

**Requires AEM 6.0**

Configure a new instance of the `com.adobe.acs.commons.logging.impl.SyslogAppender` with the host and port of your syslog server. To log all messages, leave the logger names field as `ROOT`; otherwise specify the specific logger names you want to send to the server.

![syslog configuration]({{ site.data.acs-aem-commons.baseurl }}/images/syslog/config.png)

When testing this configuration, you should verify that the remote syslog daemon accepts requests from an external source. Experience shows that, by default, syslog daemons usually deny requests coming via a network connection.