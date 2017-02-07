---
layout: default
title:  "Data Feeds"
date:   2017-02-01 10:30:15 -0600
category: "Feed Management"
type: feature
trending: true
tags: [feed, data, setup, management, source]
---

# Data Feeds

* TOC
{:toc}

## Getting started

Data feed is the core element of AdBOOST that is used to create [Product Campaigns]({% post_url 2017-01-30-product-campaigns %}), [Automated banners]({% post_url 2017-01-31-banner-generator %}) or [Exports for external networks]({% post_url 2017-01-30-feed-exports %}). It is AdBOOST's internal entity that represents data source. This entity can obtain it's data from sources in various formats:

- CSV
- TSV
- XML
- txt
- Google Spreadsheet

To get you ready for using AdBOOST, you need to have at least one data feed with your items accessible at remote URL. If you don't have it and you do not want to wait for your fellow programmers to set one up for you, you can follow instructions in [Google spreadsheet feed guide]({% post_url 2017-02-06-google-spreadsheet-feed %}) and create one yourself.

When you have your feed ready, you can proceed to AdBOOST feed creation in multiple ways:

**Welcome screen** - if do not have anything set-up in your AdBOOST account, you can create your first feed by clicking the <span class="btn btn-sm btn-primary"><i class="fa fa-plus"></i> Add first Feed</span> button on main dashboard

{% include image_tag.html url="/images/feeds/WelcomeScreen.png" alt="Welcome screen" style="" %}

**Left menu** - from any part of AdBOOST, you can go directly to new feed addition by clicking the <i class="fa fa-plus"></i> button next to the "Feeds" label in left menu.

{% include image_tag.html url="/images/feeds/LeftSidebar.png" alt="Left Sidebar" style="height:200px;" %}

**Redirects** - since at least one active feed is required to use any AdBOOST functionallity (except [Monitoring tool]({% post_url 2017-02-06-monitoring-tool %})), you will be redirected to feed setup form if you try to create any other entitites

## Feed setup workflow

- your **feed** will be **created** after successful saving of [Schema settings](#schema-settings) form
- your **items** will be **pre-fetched** after successful saving of [Filter items](#filter-items) form
- your **items** will be **imported to AdBOOST** after successful saving of [Edit items](#edit-items) form
- **feed** will be **updated with your desired frequency** after saving of [Schedule](#schedule) form

## Schema settings

Regardless of what way you choose, you will be greeted by empty feed schema form, with two required fields and tour info message explaining feed-related conventions.

{% include image_tag.html url="/images/feeds/EmptyFeedForm.png" alt="Empty Feed Form" style="" %}

When you fill in the feed name and the URL, feed schema will be generated. AdBOOST wil examine properties of items in your feed and assign them to most suitable containers. Pay special attention to **Required properties**. If you leave any of them blank, you will not be allowed to continue in feed setup.

{% include image_tag.html url="/images/feeds/RequiredFieldsFilled.png" alt="Required Fields Filled" style="" %}

If you do not want any of feed properties to be processed, just drag and drop it on the <i class="glyphicon glyphicon-trash"></i> icon.

Do not be afraid to make changes to your feed URL. Anytime you try to do so, dialog with processing options will appear and you will have another chance to change your mind about it. Dialog will be shown after URL change or after click on <i class="fa fa-refresh"></i> icon.

{% include image_tag.html url="/images/feeds/UrlReloadAction.png" alt="Url Reload Action" style="" %}

Schema itself can be divided into six parts:

### Required properties

These are properties that will be used to distinguish and identify your items and therefore:

- **ID** has to be unique. Please choose property that has lowest probability of duplicit values (EAN, ISBN, etc.)
- **Item name** will help you to differentiate your products and will be used as a display property for your Ad Groups or Export items
- **URL** has to point to web page with content related to this specific item. Otherwise, it might get rejected by target advertising network

{% include image_tag.html url="/images/feeds/RequiredProps.png" alt="Required Properties" style="" %}

### Recommended properties

Properties that will be identified by AdBOOST or can be dragged into respective container by you. You will be able to continue in setup process, even if you leave any of them blank, but every one of these properties has some role:

- **Numerical values** will be used as a replacements of {param1} and {param2} placeholders in your [Product Campaigns]({% post_url 2017-01-30-product-campaigns %}) ads
- **Category** property can later be used to segment your feed and automatically create [Batch of Campaigns]({% post_url 2017-02-06-batch-campaigns %})
- **Manufacturer** property will be used to create suggestions for your [Keyword Pattern]({% post_url 2017-02-06-keyword-patterns %}) and [Ad Patterns]({% post_url 2017-02-06-ad-patterns %})

{% include image_tag.html url="/images/feeds/RecommendedProps.png" alt="Recommended Properties" style="" %}

### Image properties

Here you should place all properties that content some image URL. They are the only ones that can be used in [Banner Generator]({% post_url 2017-01-31-banner-generator %}#image-layer) as a part of the image layer. Images from these URLs will also be pre-fetched and your future work in AdBOOST that will include them will therefore be much faster.

{% include image_tag.html url="/images/feeds/ImageProperties.png" alt="Image Properties" style="" %}

### Other numerical values

Here you should place all values that you later wish to use in [Modifier rules]({% post_url 2017-01-29-adboost-rules %}#predicates)) as a part of the condition with numeric operators (<, >, =, <=, >=).

{% include image_tag.html url="/images/feeds/OtherNumeric.png" alt="Other Numeric Values" style="" %}

### Other properties

This is the place for other feed properties that cannot be strictly categorized. This is also the place where you can create your own **virtual variables** that can be later filled in Feed Editor and used in other parts of AdBOOST.

{% include image_tag.html url="/images/feeds/VirtualVariable.png" alt="Other Properties" style="" %}

## Schema enhancements

This is the place where you can enrich your items by adding properties from [Heureka sortiment export](https://sluzby.heureka.cz/napoveda/objasneni-polozek-sortimentreportu/) such as number of competitors, popularity, etc. If you already have such an export, just drop it to the grey area in form. Otherwise you can skip this step.

{% include image_tag.html url="/images/feeds/SchemaEnhancements.png" alt="Schema Enhancements" style="" %}

## Filter items

You can further refine which items will be imported to AdBOOST from your feed by specifying Feed filter rules.

On the screen below, you can see sample rules (rules are described in detail in [AdBOOST rules guide]({% post_url 2017-01-29-adboost-rules %})) that filter 746 of 1 581 items in feed.

{% include image_tag.html url="/images/feeds/FeedItemFiltering.png" alt="Feed Item Filtering" style="" %}

Pay special attention to **Available account items quota**. It is the number of items you have left to be imported to AdBOOST. Every trial account starts with 10 000 items quota that can be later enhanced. If you exceed this limit with current filter conditions, you will be presented with warning and AdBOOST will import number of items equal to remaining quota portion (it this case 195 of 1 518)

{% include image_tag.html url="/images/feeds/UnsufficientQuota.png" alt="Unsufficient Quota" style="" %}

Last part of this form is preview of filtered item at its bottom. It shows up to 100 items and can be filtered upon by item name, id, category or URL.

{% include image_tag.html url="/images/FilteredItemsPreview.png" alt="Filtered Items Preview" style="" %}
