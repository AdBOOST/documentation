---
layout: default
title:  "Feed Setup"
date:   2017-02-01 10:30:15 -0600
category: feed_management
tags: [feed, data, setup, management, source]
---

# Feed Setup
<br/>

* TOC
{:toc}

## Getting started

Data feed is the core element of AdBOOST that is used to create [Product Campaigns]({% post_url 2017-02-06-product-campaigns %}), [Automated banners]({% post_url 2017-01-31-banner-generator %}) or [Exports for external networks]({% post_url 2017-01-30-feed-exports %}). It is AdBOOST's internal entity that represents data source. This entity can obtain it's data from sources in various formats:

- CSV
- TSV
- XML
- txt
- Google Spreadsheet

To get you ready for using AdBOOST, you need to have at least one data feed with your items accessible at remote URL. If you don't have it and you do not want to wait for your fellow programmers to set one up for you, you can follow instructions in [Google spreadsheet guide]({% post_url 2017-02-06-google-spreadsheet-feed %}) and create one yourself.

When you have your feed ready, you can proceed to AdBOOST feed creation in multiple ways:

**Welcome screen** - if do not have anything set-up in your AdBOOST account, you can create your first feed by clicking the <span class="btn btn-sm btn-primary"><i class="fa fa-plus"></i> Add first Feed</span> button on main dashboard

{% include image_tag.html url="/images/feeds/WelcomeScreen.png" alt="Welcome screen" style="" %}

**Left menu** - from any part of AdBOOST, you can go directly to new feed addition by clicking the <i class="fa fa-plus"></i> button next to the "Feeds" label in left menu.

{% include image_tag.html url="/images/feeds/LeftMenu.png" alt="Left Menu" style="" %}

**Redirects** - since at least one active feed is required to use any AdBOOST functionallity (except [Monitoring tool]({% post_url 2017-02-06-monitoring-tool %})), you will be redirected to feed setup form if you try to create any other entitites

## Schema setup

