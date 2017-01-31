---
layout: default
title:  "Feed Exports"
date:   2017-01-30 16:59:30 -0600
category: feed_management
tags: [feed, export]
---

## Feed Exports

In left context menu choose <i class="fa fa-database">&nbsp;</i> Data Management > <i class="fa fa-share">&nbsp;</i> Exports.<br/>

{% include image_tag.html url="/AdBOOST/images/exports/LeftMenuExport.png" alt="Left Menu Export" style="height:200px;" %}

If you have not created any export yet, you will be greeted by welcome screen consisting of selection of available target networks.

{% include image_tag.html url="/AdBOOST/images/exports/ExportGuidedSetup.png" alt="Export Guided Setup" style="" %}

If you have already created any feed exports, you will see them in listing and you will have the option to create new one by clicking either <span class="btn btn-sm btn-default"><i class="fa fa-plus">&nbsp;</i> Export</span> button or <span class="btn btn-sm btn-default"><i class="fa fa-question">&nbsp;</i> Guided setup</span> button

{% include image_tag.html url="/AdBOOST/images/exports/ExportListing.png" alt="Export Listing" style="" %}

Choose your target network and you will be redirected to an empty form with one input for export name and another one with selection of your feeds from which you should choose one that will be used as a data source for an export. **Both fields are required**. Source feed can be changed later in the process but if you replace it by feed with different schema, you may loose some data that you have filled into the form.

{% include image_tag.html url="/AdBOOST/images/exports/ExportEmptyForm.png" alt="Export Empty Form" style="" %}

After you have filled in first two required properties of your export, additional export settings will be shown. Properties marked with red asterisk - <span class="text-red">*</span> are required and will remain highlighted in yellow until you bound them to corresponding feed property or provide static value for them.

You can also provide feed property in combination with static value that will be used in case of missing property value for some of your feed items.

There are also "sets" of properties that require at least one of them to be set. E.g. in case of Facebook, you have to set at least one of Identifier, Brand and MPN properties. These properties are highlighted in yellow but do not have red asterisk next the title.

{% include image_tag.html url="/AdBOOST/images/exports/ExportFormProgress.png" alt="Export Form Progress" style="" %}

Some export properties can have only certain values supported by target network. It's up to you to choose feed property that fulfills these restrictions. Static values are validated automatically.

{% include image_tag.html url="/AdBOOST/images/exports/ExportStaticFieldValid.png" alt="Export Static Field Valid" style="" %}

AdBOOST allows you to map your item categories to values supported by export's target network. This feature is currently available for:

- <i class="fa fa-google google-icon-color">&nbsp;</i> Google Merchant Center [EN/CZ]
- <i class="fa fa-facebook-official facebook-icon-color">&nbsp;</i> Facebook [EN]
- <i class="network-icon heureka">&nbsp;</i> Heureka [CZ/SK]
- <i class="network-icon zbozi">&nbsp;</i> Zbozi.cz [CZ]

 If you want to use this feature, you have to select property of your items that will be used as a mapping source.

{% include image_tag.html url="/AdBOOST/images/exports/ExportCategoryMappingNotSelected.png" alt="Export Category Mapping Not Selected" style="" %}

Afterwards, you can click <span class="btn btn-sm btn-default"><i class="fa fa-wrench">&nbsp;</i> Map to {NETWORK} categories</span> button and you will see the dialog with values of selected property and inputs with fulltext search next to them. You can refine your searches until you find most suitable category supported by target network. Default value at the top of the modal will be used as a last option in case of missing feed property value, empty or unsuitable selected option.

{% include image_tag.html url="/AdBOOST/images/exports/ExportCategoryMapping.png" alt="Export Category Mapping" style="" %}

When you are satisfied with your category mapping, save the content of dialog. **If you close the dialog without saving, values will be lost**. Otherwise, you will notice that default value of attribute in main form has changed and green <i class="glyphicon glyphicon-ok">&nbsp;</i>icon has appeared in category property row to indicate that mapping is active.

{% include image_tag.html url="/AdBOOST/images/exports/ExportCategoryMappingActive.png" alt="Export Category Mapping Active" style="" %}

Feed exports for Facebook allow you to assign automated banner ads created with AdBOOST as product images. This feature is available after clicking to <span class="btn btn-sm btn-default"><i class="fa fa-image">&nbsp;</i> Assign banner templates</span> button. Whether you activate it or not, AdBOOST will choose image for your product in this order:

1. Banner templates in your priority order (if there are any)
2. Feed property selected as image property for export
3. Default value in form (URL)

{% include image_tag.html url="/AdBOOST/images/exports/FacebookBannerMapping.png" alt="Facebook Banner Mapping" style="" %}

If you want to assign banner template as a product image and you see dialog below, it means you have not created any banner template yet. In this case follow our [Banner generator]({% post_url 2017-01-31-banner-generator %}) manual to create some.

{% include image_tag.html url="/AdBOOST/images/exports/FacebookNoBanners.png" alt="Facebook No Banners" style="" %}
