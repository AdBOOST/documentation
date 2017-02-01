---
layout: default
title:  "Feed Exports"
date:   2017-01-30 16:59:30 -0600
category: feed_management
tags: [feed, export]
---

# Feed Exports
<br/>

* TOC
{:toc}

## Basic setup

In left context menu choose <i class="fa fa-database"></i> Data Management > <i class="fa fa-share"></i> Exports.<br/>

{% include image_tag.html url="/images/exports/LeftMenuExport.png" alt="Left Menu Export" style="height:200px;" %}

If you have not created any export yet, you will be greeted by welcome screen consisting of selection of available target networks.

{% include image_tag.html url="/images/exports/ExportGuidedSetup.png" alt="Export Guided Setup" style="" %}

If you have already created any feed exports, you will see them in listing and you will have the option to create new one by clicking either <span class="btn btn-sm btn-primary"><i class="fa fa-plus"></i> Export</span> button or <span class="btn btn-sm btn-primary"><i class="fa fa-question"></i> Guided setup</span> button

{% include image_tag.html url="/images/exports/ExportListing.png" alt="Export Listing" style="" %}

Choose your target network and you will be redirected to an empty form with one input for export name and another one with selection of your feeds from which you should choose one that will be used as a data source for an export. **Both fields are required**. Source feed can be changed later in the process but if you replace it by feed with different schema, you may loose some data that you have filled into the form.

{% include image_tag.html url="/images/exports/ExportEmptyForm.png" alt="Export Empty Form" style="" %}

After you have filled in first two required properties of your export, additional export settings will be shown. Properties marked with red asterisk - <span class="text-red">*</span> are required and will remain highlighted in yellow until you bound them to corresponding feed property or provide static value for them.

You can also provide feed property in combination with static value that will be used in case of missing property value for some of your feed items.

There are also "sets" of properties that require at least one of them to be set. E.g. in case of Facebook, you have to set at least one of Identifier, Brand and MPN properties. These properties are highlighted in yellow but do not have red asterisk next to the title.

{% include image_tag.html url="/images/exports/ExportFormProgress.png" alt="Export Form Progress" style="" %}

Some export properties can have only certain values supported by target network. It's up to you to choose feed property that fulfills these restrictions. Static values are validated automatically.

{% include image_tag.html url="/images/exports/ExportStaticFieldValid.png" alt="Export Static Field Valid" style="" %}

## Category mapping

AdBOOST allows you to map your item categories to values supported by export's target network. This feature is currently available for:

- <i class="fa fa-google google-icon-color"></i> Google Merchant Center [EN/CZ]
- <i class="fa fa-facebook-square facebook-icon-color"></i> Facebook [EN]
- <i class="network-icon heureka"></i> Heureka [CZ/SK]
- <i class="network-icon zbozi"></i> Zbozi.cz [CZ]

 If you want to use this feature, you have to select property of your items that will be used as a mapping source.

{% include image_tag.html url="/images/exports/ExportCategoryMappingNotSelected.png" alt="Export Category Mapping Not Selected" style="" %}

Afterwards, you can click <span class="btn btn-sm btn-default"><i class="fa fa-wrench"></i> Map to {NETWORK} categories</span> button and you will see the dialog with values of selected property and inputs with fulltext search next to them. You can refine your searches until you find most suitable category supported by target network. Default value at the top of the modal will be used as a last option in case of missing feed property value, empty or unsuitable selected option.

{% include image_tag.html url="/images/exports/ExportCategoryMapping.png" alt="Export Category Mapping" style="" %}

When you are satisfied with your category mapping, save the content of dialog. **If you close the dialog without saving, values will be lost**. Otherwise, you will notice that default value of attribute in main form has changed and green <i class="glyphicon glyphicon-ok"></i> icon has appeared in category property row to indicate that mapping is active.

{% include image_tag.html url="/images/exports/ExportCategoryMappingActive.png" alt="Export Category Mapping Active" style="" %}

## Automated banners as product images

<div class="text-red beta-notice">Feature is available only for Facebook network</div>
Feed exports for Facebook allow you to assign automated banner ads created with AdBOOST as product images. This feature is available after clicking to <span class="btn btn-sm btn-default"><i class="fa fa-image"></i> Assign banner templates</span> button. Whether you activate it or not, AdBOOST will choose image for your product in this order:

1. Banner templates in your priority order (if there are any)
2. Feed property selected as image property for export
3. Default value in form (URL)

{% include image_tag.html url="/images/exports/FacebookBannerMapping.png" alt="Facebook Banner Mapping" style="" %}

If you want to assign banner template as a product image and you see dialog below, it means you do not have any banners that are suitable for Facebook advertising network or you have not yet created any banner template at all. In this case follow our [Banner generator guide]({% post_url 2017-01-31-banner-generator %}) to create some.

{% include image_tag.html url="/images/exports/FacebookNoBanners.png" alt="Facebook No Banners" style="" %}

When you have successfully created at least one banner template, that is eligible for usage in Facebook (ratio 1:1 and minimal width 600px), content of banner template assign dialog will change to version shown on image below.

{% include image_tag.html url="/images/exports/FacebookBannersModal.png" alt="Facebook Banners Modal" style="" %}

As in case of category mapping, green <i class="glyphicon glyphicon-ok"></i> icon will be displayed in image property row to indicate that banner template assign is active, right after submit of dialog.

{% include image_tag.html url="/images/exports/FacebookBannerAssignActive.png" alt="Facebook Banners Assign Active" style="" %}

If you have set all required properties and your are satisfied with overall structure of your export, scroll to the bottom of the page and click one of submit buttons:

- Save & export - saves the export schema, creates export itself and refreshes the page
- Save & go to next step - does same as the first button but navigates to item filtering after successfull save

{% include image_tag.html url="/images/exports/ExportSubmitBtns.png" alt="Export Submit Buttons" style="" %}

## Export status

No matter what option you choose, every screen of export setup will contain status label and URL after first schema submit. **URL is persistent. Once it has been generated, it will forever refer to this specific export**. If there are some changes in schema, category mapping, assigned banner templates or in feed data, export will be re-processed and this URL will always contain most up-to-date version.

{% include image_tag.html url="/images/exports/ExportStatusLabel.png" alt="Export Status Label" style="" %}

Status label is an indicator of export health and can have following states:

{% include image_tag.html url="/images/StatusLabelStates.png" alt="Status Label States" style="" %}

It always contains state information and action button. Click to <i class="fa fa-refresh"></i> icon starts re-processing of export and click to <i class="fa fa-clock-o"></i> icon shows dialog displayed below which contains information about export processing history, corresponding issues and recovers.

{% include image_tag.html url="/images/exports/ExportProcessingLog.png" alt="Export Processing Log" style="" %}

## Item filtering

You can further refine which items will be exported by specifying Export filter rules. Your items are then processed by AdBOOST in following order:

1. **Feed filter rules** - control which items enter AdBOOST
2. **Feed editor rules** - modify and purge your items
3. **Export filter rules** - control which items will be part of the export (you can have more exports bound to one feed that differ only by filter rules)
4. **Export CPC edit rules** (optional) - currently available only for Heureka and later described in [Automated bidding part](#automated-bidding)

On the screen below, you can see sample rules (rules are described in detail in [AdBOOST rules guide]({% post_url 2017-02-01-adboost-rules %})) that filter 746 of 1 581 items in feed.

{% include image_tag.html url="/images/exports/ExportItemFiltering.png" alt="Export Item Filtering" style="" %}

Notice also the counter of item categories that are suitable for provided rules with <i class="glyphicon glyphicon-search pointer"></i> icon next to it. By clicking this icon, you will invoke displaying of dialog with list of these categories, that can be later filtered upon.

{% include image_tag.html url="/images/FilterRulesCategoryPreview.png" alt="Filter Rules Category Preview" style="" %}

Last part of this form is preview of filtered item at its bottom. It shows up to 100 items and can be filtered upon by item name, id, category or URL.

{% include image_tag.html url="/images/FilteredItemsPreview.png" alt="Filtered Items Preview" style="" %}

## Automated bidding

<div class="text-red beta-notice">Feature is available only for Heureka network</div>
Last part of export setup, which is currently available only for Heureka network, allows you to automate your CPC values and reflect changes in your feed hourly. Thanks to this feature, you can optimize your advertising spend by covering many cases. Here are just a few most common examples:

- Do not set CPC too high for items with low price

{% include image_tag.html url="/images/exports/ExportBidding1.png" alt="Export Bidding 1" style="" %}

- Sell out stock quickly to free your warehouse space for fresh (seasonal) merchandise

{% include image_tag.html url="/images/exports/ExportBidding2.png" alt="Export Bidding 2" style="" %}

- Restrict your maximum CPC to fulfill requirements of target network. If you set CPC to certain fragment of item price, it might be too high for expensive items

{% include image_tag.html url="/images/exports/ExportBidding3.png" alt="Export Bidding 3" style="" %}

