---
layout: default
title:  "Monitoring tool"
date:   2017-02-06 09:28:14 -0600
category: "Monitoring Tool"
type: feature
tags: [google, adwords, facebook, heureka, sklik, analytics, seznam, client, account, performance, report, campaign, monitoring]
---

# Monitoring tool

* TOC
{:toc}

## Getting started

Monitoring tool is a part of AdBOOST that can be used to watch performance of your client accounts across multiple networks. For the sake of simplicity, it consists of two screens which you can use to identify potential performance issues and avoid them before they actually arise.

To explore its functionallity choose <i class="fa fa-area-chart"></i> Monitoring > <i class="fa fa-user"></i> Clients in left context menu<br/>

{% include image_tag.html url="/images/monitoring/LeftMenu.png" alt="Left Menu" style="height:200px;" %}

## Client Form

If you do not already posses access rights to any monitoring client account, you will be presented with screen consisting of help text describing monitoring entities and client setup process.

Below this help text, you can find the client form. Give name to your client (required) and tag it for better identification (optional and can be done later). Afterwards you can click the <span class="btn btn-sm btn-primary"><i class="fa fa-save"></i> Save</span> button and proceed to advertising channels setup.

{% include image_tag.html url="/images/monitoring/EmptyClientForm.png" alt="Empty Client Form" style="" %}

## Advertising Channels

Every monitoring client account is perceived as a set of **advertising channels**. To activate a channel for your client, you need to perform following steps:

- click the <span class="btn btn-sm btn-default"><i class="fa fa-link"></i> Link {NETWORK}</span> button to verify your current AdBOOST e-mail with OAUTH - **only for Google and Facebook**
- provide your client identifier - to find out where you should look after the client identifier across multiple network interfaces, please refer to chapter [Client Identifiers](#client-identifiers)
- set currency for your channel. Channels will be later grouped by currency for cummulative statistics reports
- wait for icon in **Checked** column to turn into the green <i class="glyphicon glyphicon-ok"></i> mark and click the Save button. It will also turn green after successful channel save

Every element in this form has a tooltip, so if you wonder what it does, just hover over it with mouse cursor.

{% include image_tag.html url="/images/monitoring/ClientWithDefaultsForm.png" alt="Client With Defaults Form" style="" %}

Channels setup itself can include another three specific tasks:

* tick checkbox in "Active" column if you wish to PAUSE advertising **channel that has already been saved**. Afterwards, you should confirm your action with click to Save buttton. Otherwise, manipulation with this element will not have any effect
* if you are a part of an AdBOOST Agency that already has some shared e-mail addresses that have been verified with OAUTH, you will see them listed in dropdown in **Linked Accounts** column. You can still verify your current e-mail by clicking the <i class="fa fa-plus"></i> icon. If you do not wish to do so, you can choose one of available e-mails from dropdown. Only important thing is to **choose the e-mail that is used as an owner in account with provided identifier**
* if you decide to activate an Analytics channel, you still have to provide account identifier to check account connectivity. After its verification, you will be presented with two dropdowns:

    1. **Property ID** - segment of your analytics account e.g. language versions of same website
    2. **View ID** - event set within account segment defined by you. Default value equals to "All website data"

{% include image_tag.html url="/images/monitoring/ClientEditModal.png" alt="Client Edit Modal" style="" %}

## Client Identifiers


