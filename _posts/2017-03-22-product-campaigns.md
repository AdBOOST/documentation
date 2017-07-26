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

{% include image_tag.html url="/images/campaigns/BingAdvertisingPolicies.png" alt="Bing Advertising Policies" style="height:100px;" %}

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

#### General settings

First thing to choose is the name of your campaign and the feed that will be used as a data source for campaign ads and keywords.

{% include image_tag.html url="/images/campaigns/SklikGeneralSettings.png" alt="Sklik General Settings" style="" %}

Please pay attention to the label next to the campaign name input. Name you choose for your campaign won't be final as it will be used according to naming conventions set in account settings form.

{% include image_tag.html url="/images/campaigns/NamingConventions.png" alt="Naming Conventions" style="" %}

Other campaign settings include setting of daily budget and default campaign bid. Ticking of "Ignore item bid update" checkbox leaves bid management to you and won't override values provided in Sklik interface with those set in AdBOOST.

{% include image_tag.html url="/images/campaigns/SklikCampaignSettings.png" alt="Sklik Campaign Settings" style="" %}

Advertising policies part of the form is the place where you can set autocorrect rules for punctuation and font case in ads. You can also set the ad selection policy, so they will be rotated the way that suits you best.

{% include image_tag.html url="/images/campaigns/SklikAdvertisingPolicies.png" alt="Sklik Advertising Policies" style="height:100px;" %}

## Item assignment

Campaign assign items form determines which items from the campaign's source data feed will be used to create ads and keywords. This form consist of following parts.

First of all, you can examine categories of products in source data feed in tree structure placed in "Item categories" container.

{% include image_tag.html url="/images/campaigns/AssignCategoryTree.png" alt="Assign Category Tree" style="" %}

Core part of the form consists of rule container where you can specify your predicates and conditions for item filtering. To find out more about AdBOOST rules, please refer to our [AdBOOST rules guide]({% post_url 2017-01-29-adboost-rules %}). To see how many items from feed you have selected to fit into this campaign, refer to counters on the right side of form.

{% include image_tag.html url="/images/campaigns/AssignFormCore.png" alt="Assign Form Core" style="" %}

Items can be examined deeper in preview container. Use the input at the top of the container to filter items in preview by name, id or category. You will see up to 100 matched items and counter showing overall number of matched items.

{% include image_tag.html url="/images/campaigns/AssignedItemsPreview.png" alt="Assigned Items Preview" style="" %}

If you are also curious which item categories will be covered by this selection, click the <i class="glyphicon glyphicon-search"></i> icon in the "Number of items assigned from feed" container and you will see filterable view of matched categories.

{% include image_tag.html url="/images/campaigns/AssignedCategoriesPreview.png" alt="Assigned Categories Preview" style="" %}

## Keyword patterns

Next step in campaign creation process is the specification of keyword patterns. This part of campaign can be managed either after the click to the "Keyword patterns" action in campaigns listing or after the selection of the "Keyword patterns" tab in the campaign setup process.

{% include image_tag.html url="/images/patterns/KpFormLinks.png" alt="Keyword Pattern Form Links" style="" %}

In case of campaign with some existing keyword patterns, the form can be accessed by click to the <span class="btn btn-sm btn-primary"><i class="glyphicon glyphicon-plus-sign"></i> Keyword pattern</span> button in the keyword patterns listing.

{% include image_tag.html url="/images/patterns/AddKeywordPatternButton.png" alt="Add Keyword Pattern Button" style="" %}

If you haven't created any patterns yet, you will be redirected straight to the new Keyword pattern form.

{% include image_tag.html url="/images/patterns/EmptyKpForm.png" alt="Empty Keyword Pattern Form" style="" %}

You only have to provide patterns for your keywords and match typeof resulting keywords in order to save the form. As you can notice, keywords patterns are inserted in one-per-line manner. Keywords name is optional and will only help you to better recognize your pattern in the listings.

Match type option follows the target network rules. You can therefore choose to create keywords as exact, phrase or broad. Enhancement broad to you by AdBOOST is the possibility to create keywords in all matches at one by selecting the "ALL" option.

{% include image_tag.html url="/images/patterns/KpMatchType.png" alt="Keyword Pattern Match Type" style="" %}

As mentioned previously, in case of new form, patterns are provided one-per-line, what is immediately reflected in the preview

{% include image_tag.html url="/images/patterns/OnePerLinePreview.png" alt="One Per Line Preview" style="" %}

Preview can be also inspected in the batch modal where you can define how many products per size you want to see. Batch preview is accessed by click to the <i class="glyphicon glyphicon-tasks"></i> icon and as displayed on the image below, patterns are ordered as they are on the input.

{% include image_tag.html url="/images/patterns/KpBatchPreview.png" alt="Keyword Pattern Batch Preview" style="" %}

Preview can be later refined by specifying the filter value which will consider product's name, id and category.

{% include image_tag.html url="/images/patterns/KpProductPreview.png" alt="Keyword Pattern Product Preview" style="height:350px;" %}

Keyword modifiers will allow you to perform following actions:

- generate only keywords of certain length (e.g. from 2 to 5 words)
- generate all keywords but trim result to max X characters
- exclude phrases from generated keywords (before the length modifiers are applied)

{% include image_tag.html url="/images/patterns/KeywordModifiers.png" alt="Keyword Modifiers" style="" %}

Last part of the pattern form allows you to one last time refine which products will use this keyword pattern to create keywords. Right side of this element allows you to choose the action for the products that are suitable for current campaign but do not fulfill provided filter rules.

{% include image_tag.html url="/images/patterns/OnFilterAction.png" alt="On Filter Action" style="" %}

If you submit the form using the <span class="btn btn-sm btn-default">Submit & Show the listing</span> button, you will be redirected to the keyword pattern listing, where you can examine properties of all keyword patterns available in current campaign. This includes all pattern properties, but these are especially useful:

- keyword pattern structure
- preview of generated keywords
- filtered/total product count
- preview of filter rules
- minimum/maximum keyword length
- number of products not covered by the pattern (calculated after the synchronisation)

{% include image_tag.html url="/images/patterns/KeywordPatternSmartFeatures.png" alt="Keyword Pattern Smart Features" style="" %}

If you submit the form using the <span class="btn btn-sm btn-primary">Submit & Go to Next Step</span> button, you will be redirected to the ad pattern form, which is covered in detail in the next section.

## Ad patterns

Now that your campaign contains the keywords that will trigger the displaying of an ad, let's create some, so there is something to show to your customers.

In case of campaign with some existing ad patterns, the form can be accessed by click to the <span class="btn btn-sm btn-primary"><i class="glyphicon glyphicon-plus-sign"></i> Ad pattern</span> button in the ad patterns listing.

{% include image_tag.html url="/images/patterns/AddAdPatternButton.png" alt="Add Ad Pattern Button" style="" %}

If you haven't created any patterns yet, you will be redirected straight to the new Ad pattern form.

{% include image_tag.html url="/images/patterns/EmptyApForm.png" alt="Empty Ad Pattern Form" style="" %}

Quickest way how you can save the ad pattern is to provide headlines and description for the first ad pattern alternative. This is the required minimum. Other settings will be explained in following paragraphs.

{% include image_tag.html url="/images/patterns/AdPatternFormFilled.png" alt="Ad Pattern Form Filled" style="" %}

Choose a **name for your ad pattern**. This will be displayed in all listings and will help you to identify it.

If your web URLs differ for different devices, you have a possibility to provide **final ad URL specific for the mobile devices**.

To compose an ad pattern, use the "Feed variables" box at the left side of the form and **drag&drop the variables** you wish ot show in your adverts. You can also insert some static text. **Counters above the inputs are re-calculated in the real-time**. They will tell you, whether the items that entered this ad pattern alternative, fit the target network's ad text length requirements.

**Arrows with counters** will tell you how many of your products are used as an input for the alternative, how many of them are eligible to create an ad and how many of them will have to be examined by the next one.

Easiest way how you can create all alternatives and cover as many products as possible, is to create the first one, click the **"Copy" arrow** and adjust the next alternative, so it will have no products on the output.
