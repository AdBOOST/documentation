---
layout: default
title:  "Product Campaigns"
date:   2017-03-22 17:10:41 -0600
category: "Product Campaigns"
type: feature
tags: [google, adwords, network, campaign, product, ppc, bing, bingads, yahoo, sklik, seznam, ad, keyword]
---

# Product Campaigns

* TOC
{:toc}

## Getting started

Only pre-requisity of product campaigns setup is to have at least one active data feed in AdBOOST. If you do not have one yet, please follow our [Feed setup guide]({% post_url 2017-02-01-data-feeds %})

## Basic setup

In left context menu choose <i class="fa fa-bullhorn"></i> Product Campaigns > <i class="fa fa-dashboard"></i> Dashboard or click to large "<i class="fa fa-bullhorn"></i> Product campaigns" icon <br/> on the main dashboard<br/>

{% include image_tag.html url="/images/campaigns/LeftMenuCampaigns.png" alt="Left Menu Campaigns" style="height:350px;" %}

If you have not created any product campaign yet, you will be greeted by product campaigns dashboard with info message about features that you currently do not use. As you can notice, there are three ways how you can proceed to new campaign addition. Two <i class="fa fa-plus"></i> buttons (one next to the Product Campaigns link and second next to "Campaigns" in left menu) and one **Create your first Campaign** link. All of them will redirect you to the campaign form.

{% include image_tag.html url="/images/campaigns/EmptyCampaignsDashboard.png" alt="Empty Campaigns Dashboard" style="" %}

Here you can choose which way do you want to go:
- if you want to create your campaigns really quickly and you do not care so much about them being generic, forget this tutorial and continue with our [Batch Campaign Creator guide]({% post_url 2017-03-23-batch-campaigns %}).
- if you want to create the display campaign for Google Display Network, continue with our [Google Display Campaigns guide]({% post_url 2017-02-01-google-display-campaigns %})
- otherwise choose one of the target advertising networks

{% include image_tag.html url="/images/campaigns/GuidedSetup.png" alt="Guided Setup" style="" %}

## Campaign Settings

These settings might consist of 1-2 steps and differ slightly for each target advertising network.

### AdWords

#### General settings

First thing to choose is the name of your campaign and the feed that will be used as a data source for campaign ads and keywords.

{% include image_tag.html url="/images/campaigns/AwGeneralSettings.png" alt="Aw General Settings" style="" %}

Please pay attention to the label next to the campaign name input. Name you choose for your campaign won't be final as it will be used according to naming conventions set in account settings form.

{% include image_tag.html url="/images/campaigns/NamingConventions.png" alt="Naming Conventions" style="" %}

Later you will be prompted to provide campaign budget to limit amount of money available to this campaign. You can choose from two options:

- **Dedicated budget** that will be available only to this specific campaign and can be managed only in this form,
- **Shared budget** that could be re-used accross your campaigns and can also be managed in Shared library

{% include image_tag.html url="/images/campaigns/AwBudgetSettings.png" alt="Aw Budget Settings" style="" %}

If you find out that none of your existing shared budgets fits needs of this campaign, you can create new one in the dialog shown after click to <span class="btn btn-sm btn-default"><i class="glyphicon glyphicon-plus-sign"></i> Create new</span> button next to the shared budgets selectbox.

{% include image_tag.html url="/images/campaigns/AwCreateBudget.png" alt="Aw Create Budget" style="" %}

As mentioned before, all shared budgets can also be managed in **Shared library** that can be examined in left context menu under Product Campaigns after click to the caret next to the Shared Library label.

{% include image_tag.html url="/images/campaigns/LeftMenuBudgets.png" alt="Left Menu Budgets" style="" %}

Next thing to set-up are campaign's bidding options. In case of AdWords campaigns, you can control your bidding in three ways:

- set **default campaign bid**. This value can later be overriden on keyword pattern level,
- choose the manner in which your bidding will progress - your **bidding schema**. Default value resolves to Manual CPC
- fallback that can be used in case that you want to make manual modification to the bidding setup of your specific adgroups. Normally, these are overriden but you can ommit this behavior be ticking this checkbox

{% include image_tag.html url="/images/campaigns/AwBiddingSettings.png" alt="Aw Bidding Settings" style="" %}

Again, you can create new bidding schemas in the dialog shown after click to <span class="btn btn-sm btn-default"><i class="glyphicon glyphicon-plus-sign"></i> Create new</span> button next to the bidding schemas selectbox and all your account bidding schemas can be managed in Shared library.

{% include image_tag.html url="/images/campaigns/AwCreateSchema.png" alt="Aw Create Schema" style="" %}

Ad settings section of this form has only two parts:

- **ad rotation** determines way how your ads are shown to your customers. Options speak for themselves
- you can also **request trademark exemption** in case you know that your ads will contain trademarks that you are eligible to use in AdWords advertising

{% include image_tag.html url="/images/campaigns/AwAdSettings.png" alt="Aw Ad Settings" style="" %}

Last part of General settings is UTM tagging setup. UTM tagger is generic, re-usable component of AdBOOST and you can find it on multiple levels. To find out more about how UTM tagging works and where it can be set, please refer to our [UTM tagger guide]({% post_url 2017-03-20-utm-tagger %})

#### Targeting

You can refine targeting of your AdWords campaigns in three ways:

**Preserve AdWords settings** - as you can see on the screen below, you can leave AdBOOST out of your targeting setting flow and manage this part of your campaigns in AdWords alone. Use this option at your own risk.

{% include image_tag.html url="/images/campaigns/AwPreserveTargeting.png" alt="Aw Preserve Targeting" style="" %}

**Target specific languages** - choose one or more languages supported by AdWords. Input works as a fulltext search and language names are in english.

{% include image_tag.html url="/images/campaigns/AwTargetLanguage.png" alt="Aw Target Language" style="" %}

**Target specific locations** - not only you can target specific country, district or city, you can also modify bidding in these areas according to your needs. This way you can bid more in locations where you have to deal with local competitor or less in locations that are not so popular etc.

{% include image_tag.html url="/images/campaigns/AwTargetLocation.png" alt="Aw Target Location" style="" %}

### Bing Ads

#### General settings

First thing to choose is the name of your campaign and the feed that will be used as a data source for campaign ads and keywords.

{% include image_tag.html url="/images/campaigns/BingGeneralSettings.png" alt="Bing General Settings" style="" %}

Please pay attention to the label next to the campaign name input. Name you choose for your campaign won't be final as it will be used according to naming conventions set in account settings form.

{% include image_tag.html url="/images/campaigns/NamingConventions.png" alt="Naming Conventions" style="" %}

Other campaign settings include setting of budget amount and type, default campaign bid, you timezone (for the synchronisation timing purposes) and required campaign description field.

{% include image_tag.html url="/images/campaigns/BingCampaignSettings.png" alt="Bing Campaign Settings" style="" %}

You can request exemption for displaying of trademarks you own in advertising policies part of the form.

{% include image_tag.html url="/images/campaigns/BingAdvertisingPolicies.png" alt="Bing Advertising Policies" style="" %}

Last part of General settings is UTM tagging setup. UTM tagger is generic, re-usable component of AdBOOST and you can find it on multiple levels. To find out more about how UTM tagging works and where it can be set, please refer to our [UTM tagger guide]({% post_url 2017-03-20-utm-tagger %})

#### Targeting

You can refine targeting of your BingAds campaigns in three ways:

**Preserve BingAds settings** - as you can see on the screen below, you can leave AdBOOST out of your targeting setting flow and manage this part of your campaigns in BingAds alone. Use this option at your own risk.

{% include image_tag.html url="/images/campaigns/BingPreserveTargeting.png" alt="Bing Preserve Targeting" style="" %}

**Target specific languages** - choose **exactly one** language supported by BingAds. Input works as a fulltext search and language names are in english.

{% include image_tag.html url="/images/campaigns/BingTargetLanguage.png" alt="Bing Target Language" style="" %}

**Target specific locations** - not only you can target specific country, district or city, you can also modify bidding in these areas according to your needs. This way you can bid more in locations where you have to deal with local competitor or less in locations that are not so popular etc.

{% include image_tag.html url="/images/campaigns/BingTargetLocation.png" alt="Bing Target Location" style="" %}

### Sklik.cz


## Item assignment


## Keyword patterns


## Ad patterns
