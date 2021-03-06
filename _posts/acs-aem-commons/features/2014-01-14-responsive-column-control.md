---
layout: acs-aem-commons_feature
title: Responsive Column Control
description: Give your authors maximal column layout flexibility.
date: 2014-01-14
thumbnail: /images/responsive-column-control/thumbnail.png
feature-tags: component-dev
tags: acs-aem-commons-features
categories: acs-aem-commons features
initial-release: 1.5.0
---

# Purpose

This generic column control component allows authors to define column widths as a percentage.

![Responsive Column Control Dialog]({{ site.data.acs-aem-commons.baseurl }}/images/responsive-column-control/dialog.png)


# How to Use

1. Ensure that *either* the `acs-commons.components` client library is embedded into your site's client library or the `acs-commons.main` client library is included on your pages (this library embeds `acs-commons.components`).
2. Enable the "Responsive Column Control" component using Design Mode.

## Notes

**Before removing columns**, delete or move any components from these columns. Once a column is deleted, any component data placed in deleted columns will persist in CRX, however it will be inaccessible to authors and end users, requiring application support team to delete. 