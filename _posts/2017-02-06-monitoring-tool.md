---
layout: default
title:  "Monitoring tool"
date:   2017-02-06 09:28:14 -0600
category: "Monitoring Tool"
type: feature
trending: true
tags: [google, adwords, facebook, heureka, sklik, analytics, seznam, client, account, performance, report, campaign, monitoring]
---

# Monitoring tool

* TOC
{:toc}

## Getting started

Monitoring tool is a part of AdBOOST that can be used to watch performance of your client accounts across multiple networks. For the sake of simplicity, it consists of two screens which you can use to identify potential performance issues and avoid them before they actually arise.

To explore its functionallity choose <i class="fa fa-area-chart"></i> Monitoring > <i class="fa fa-user"></i> Clients in left context menu or click to large "<i class="fa fa-area-chart"></i> Monitoring tool" icon <br/> on the main dashboard

{% include image_tag.html url="/images/monitoring/LeftMenu.png" alt="Left Menu" style="height:350px;" %}

## Client Form

If you do not already posses access rights to any monitoring client account, you will be presented with screen consisting of help text describing monitoring entities and client setup process.

Below this help text, you can find the client form. Give name to your client (required) and tag it for better identification (optional and can be done later). Afterwards you can click the <span class="btn btn-sm btn-primary"><i class="fa fa-save"></i> Save</span> button and proceed to advertising channels setup.

{% include image_tag.html url="/images/monitoring/EmptyClientForm.png" alt="Empty Client Form" style="" %}

## Advertising Channels

Every monitoring client account is perceived as a set of **advertising channels**. To activate a channel for your client, you need to perform following steps:

- click the <span class="btn btn-sm btn-default"><i class="fa fa-link"></i> Link {NETWORK}</span> button to verify your current AdBOOST e-mail with OAUTH - **only for Google and Facebook**
- provide your client identifier - to find out where you should look after the client identifier across multiple network interfaces, please refer to chapter [Client Identifiers](#client-identifiers)
- set currency for your channel. Channels will be later grouped by currency for cummulative statistics reports
- wait for icon in **Checked** column to turn into the green <i class="glyphicon glyphicon-ok text-green"></i> mark and click the Save button. It will also turn green after successful channel save

Every element in this form has a tooltip, so if you wonder what it does, just hover over it with mouse cursor.

{% include image_tag.html url="/images/monitoring/ClientWithDefaultsForm.png" alt="Client With Defaults Form" style="" %}

Channels setup itself can include another three specific tasks:

- tick checkbox in "Active" column if you wish to PAUSE advertising **channel that has already been saved**. Afterwards, you should confirm your action with click to Save buttton. Otherwise, manipulation with this element will not have any effect
- if you are a part of an AdBOOST Agency that already has some shared e-mail addresses that have been verified with OAUTH, you will see them listed in dropdown in **Linked Accounts** column. You can still verify your current e-mail by clicking the <i class="fa fa-plus"></i> icon. If you do not wish to do so, you can choose one of available e-mails from dropdown. Only important thing is to **choose the e-mail that is used as an owner in account with provided identifier**
- if you decide to activate an Analytics channel, you still have to provide account identifier to check account connectivity. After its verification, you will be presented with two dropdowns:

    1. **Property ID** - segment of your analytics account e.g. language versions of same website
    2. **View ID** - event set within account segment defined by you. Default value equals to "All Web Site Data"

{% include image_tag.html url="/images/monitoring/ClientEditModal.png" alt="Client Edit Modal" style="" %}

## Client Identifiers

You should provide at least one account identifier during the setup of your monitoring client.

{% include image_tag.html url="/images/MonitoringAccounts.png" alt="Monitoring Accounts" style="" %}

To get to know how to manage connections of AdBOOST to external advertising networks and where to find these identifiers, please refer to [External Advertiser Accounts guide]({% post_url 2017-02-26-external-advertiser-accounts %})

## Clients Listing

All clients you add will be shown in clients listing. As you can observe on the screen below, it mainly shows info about budget, cost and cost estimate. These metrics have following meaning:

- **Budget** - constraint set by you at the beginning of the month to have control over your spends. Other two metrics are afterwards validated against this value and columns are highlighted as you can see on the screen below.
- **Cost Estimate** - estimated cost calculated by AdBOOST. Final number is based on the historical data and this value should warn you before actual cost exceeds your budget
- **Cost** - actual cost of your advertising

All values are summed per currency for every client. Expand the table row to see individual values, shrink the row to see cummulative values (budget is an exemption as if one active channel is missing the budget, n/a will be shown as a cummulative value).

{% include image_tag.html url="/images/monitoring/ClientsListing.png" alt="Clients Listing" style="" %}

Your clients can be sorted by severity of their issues in following order:

1. **Depleted budget** - Budget and Cost estimate columns marked <span class="text-red">red</span>
2. **Estimated cost lower than 50% of budget** - Cost estimate column marked <span class="text-red">red</span>
3. **Estimated cost between 50% and 75% of budget** - Cost estimate column marked <span class="text-orange">orange</span>
4. **Estimated cost between 75% and 100% of budget** - Budget and Cost estimate columns marked <span class="text-green">green</span>

### Budget management

When you click the <i class="fa fa-edit"></i> icon in the budget column, you will be presented with dialog containing the history of your budgets and input where you can align your current month budget.

{% include image_tag.html url="/images/monitoring/BudgetModal.png" alt="Budget Modal" style="" %}

## Clients Charts

This interface allows you to inspect the performance of your client accounts and cross-validate it between multiple channels. You can control what is being fetched into your charts by following means:

- filter your clients by name
- filter your clients by tags
- select date range for which you want to inspect your stats. Use either whole number in previous days input or date range from datepicker
- select combination of channels. If none of them is selected, all of them will be displayed
- select combination of metrics for selected channels. Metrics with currency will inherit value provided for their channel. Metrics whose values range between 0 and ~2 will be scaled on separate axis to provide you with better comparison

{% include image_tag.html url="/images/monitoring/ClientCharts.png" alt="Client Charts" style="" %}

## Access Control

If you are the owner of your current AdBOOST Agency, you should see an <i class="fa fa-lock"></i> Access icon at the top of every Monitoring tool screen. This icon opens a dialog where you can manage permissions for your monitoring clients.

{% include image_tag.html url="/images/monitoring/AccessControlElement.png" alt="Access Control Element" style="" %}

In dialog itself, you can choose agency that will be subject to modifications, e-mail of your coleague which you want to be able to monitor performance of some client. When you leave the e-mail input, you will be presented with list of monitoring clients that exist within selected agency. Choose as many clients as you want, and submit your selection with click to the Save button.

{% include image_tag.html url="/images/monitoring/AccessControl.png" alt="Access Control" style="" %}
