---
layout: default
title:  "Batch Campaign Creator"
date:   2017-02-06 17:11:14 -0600
category: "Product Campaigns"
type: feature
tags: [google, adwords, sklik, seznam, batch, automated, campaign, create, pattern, target, bid, budget, sync]
---

# Batch Campaign Creator

* TOC
{:toc}

## Getting started

Only pre-requisity of batch campaign creator is to have at least one active data feed in AdBOOST. If you do not have one yet, please follow our [Feed setup guide]({% post_url 2017-02-01-data-feeds %}).

## Where to find it

You can proceed towards the AdBOOST batch campaign creator in multiple ways:

### Guided setup dialog

**Left menu** - from any part of AdBOOST, you can go directly to batch campaign creator by clicking the <i class="fa fa-plus"></i> button next to the "Campaigns" label in the left menu

{% include image_tag.html url="/images/batch_campaigns/LeftMenuCampaigns.png" alt="Left Menu Campaigns" style="height:350px;" %}

**Dashboards** - click the large "<i class="fa fa-bullhorn"></i> Product campaigns" icon <br/> on the main dashboard and continue with click to the <i class="fa fa-plus"></i> icon on the product campaigns dashboard.

{% include image_tag.html url="/images/batch_campaigns/PpcDashboard.png" alt="PPC Dashboard" style="" %}

**Campaigns listing** - in left context menu choose <i class="fa fa-bullhorn"></i> Product Campaigns > <i class="fa fa-cogs"></i> Campaigns and continue with click to <span class="btn btn-sm btn-primary"><i class="fa fa-question"></i> Guided setup</span> button

{% include image_tag.html url="/images/batch_campaigns/CampaignsListing.png" alt="Campaigns Listing" style="" %}

Next step is to choose the source feed in selectbox in guided setup dialog and click the button above it.

{% include image_tag.html url="/images/batch_campaigns/GuidedSetup.png" alt="Guided Setup" style="" %}

### Source feed links

**Feeds listing** - in left context menu choose <i class="fa fa-database"></i> Feed Management > <i class="fa fa-files-o"></i> Feeds. Select one feed, that you want to use as a source for your campaigns and in its table actions choose <i class="fa fa-puzzle-piece"></i> Batch Campaign Create

{% include image_tag.html url="/images/batch_campaigns/FeedsListing.png" alt="Feeds Listing" style="" %}

**Feed tabs** - if you have saved an editor form of your feed (refer to [Feed setup guide]({% post_url 2017-02-01-data-feeds %}#edit-items)), you can click the "Create campaigns" tab at the top of the feed setup at any time and get directly to the batch campaign creator. Or you can use the quick-link at the end of the setup flow, in the schedule form.

{% include image_tag.html url="/images/batch_campaigns/ScheduleLinks.png" alt="Schedule Links" style="" %}

## Campaigns structure

First thing to set up is how your product will be segmented into the campaigns. Setup process will not progress until you choose at least one campaign to create.

{% include image_tag.html url="/images/batch_campaigns/EmptyCampaignForm.png" alt="Empty Campaign Form" style="" %}

Tree of your categories that you could see on the previous screen has been based on the values of your **Category** property in your feed schema settings. If you do not see your categories, assign correct feed variable into this property.

{% include image_tag.html url="/images/batch_campaigns/FeedCategory.png" alt="Feed Category" style="height:350px;" %}

You can play with the segmentation depth and when you click the <span class="btn btn-sm btn-default"><i class="fa fa-sitemap"></i> Examine</span> button, your categories will be segmented into the selected depth. Below you can see two examples. First takes all unique category values as categories itself and second one descends to depth of three and allows you to wrap products from categories like "Board games" into the single campaign.

{% include image_tag.html url="/images/batch_campaigns/SegmentationDepth.png" alt="Segmentation Depth" style="" %}

You will not be able to save this form until it is not in the valid state. As you can see on the screen below, there are different types of validations that will guide you through the setup process without any mistake:

- if you choose to select at least one campaign for one of the target networks (AdWords, Sklik), their default values will be cross-validated
- cross-validation means that default bid has to be lower that the default budget and they both have to follow the rules of the network for min/max values. Same applies to the specific campaign bids and budgets and if your decide to provide only one of specific values, it will be validated against its default equivalent (specific bid & default budget and so on)
- campaign name pattern has to contain %NW% and %CATEGORY%/%FULL_CATEGORY% placeholders to ensure that final campaign names will be **unique**

{% include image_tag.html url="/images/batch_campaigns/FormValidation.png" alt="Form Validation" style="" %}

In case of AdWords defaults, inputs for target languages and locations work as auto-complete fields, so just start typing any country and language you wish to display your ads for and choose one of the suggestions. All values are in english.

{% include image_tag.html url="/images/batch_campaigns/Targeting.png" alt="Targeting" style="height:300px;" %}

Below you can see an example of the valid campaigns structure form. Submit button is enabled, targetings are provided and all bid/budget pairs are cross-valid for each of selected networks.

{% include image_tag.html url="/images/batch_campaigns/ValidForm.png" alt="Valid Form" style="" %}

If you proceed with click to the <span class="btn btn-sm btn-primary"><i class="fa fa-save"></i> Check summarization & go to pattern setup</span> button, you will be presented with summarization of your campaigns structure.

{% include image_tag.html url="/images/batch_campaigns/CampaignsReceipt.png" alt="Campaigns Receipt" style="" %}
