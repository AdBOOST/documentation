---
layout: default
title:  "Feed Exports"
date:   2017-01-30 16:59:30 -0600
category: feed_management
tags: [feed, export]
---

## Feed Exports

In left context menu choose <i class="fa fa-database">&nbsp;</i> Data Management > <i class="fa fa-share">&nbsp;</i> Exports.<br/>
<a href="/AdBOOST/images/exports/LeftMenuExport.png" data-lightbox="LeftMenuExport" data-title="Left Menu Export">
    <img src="/AdBOOST/images/exports/LeftMenuExport.png" alt="Left Menu Export" height="200">
</a>

If you have not created any export yet, you will be greeted by welcome screen consisting of selection of available target networks.
![ExportGuidedSetup](/AdBOOST/images/exports/ExportGuidedSetup.png)

If you have already created any feed exports, you will see them in listing and you will have the option to create new one by clicking either "<i class="fa fa-plus">&nbsp;</i> Export" button or "<i class="fa fa-question">&nbsp;</i> Guided setup" button
![ExportListing](/AdBOOST/images/exports/ExportListing.png)

Choose your target network and you will be redirected to an empty form with one input for export name and another one with selection of your feeds from which you should choose one that will be used as a data source for an export. **Both fields are required**. Source feed can be changed later in the process but if you replace it by feed with different schema, you may loose some data that you have filled into the form.
![ExportEmptyForm](/AdBOOST/images/exports/ExportEmptyForm.png)

After you have filled in first two required properties of your export, additional export settings will be shown. Properties marked with red asterisk - <span class="text-red">*</span> are required and will remain highlighted in yellow until you bound them to corresponding feed property or provide static value for them.

You can also provide feed property in combination with static value that will be used in case of missing property value for some of your feed items.

There are also "sets" of properties that require at least one of them to be set. E.g. in case of Facebook, you have to set at least one of Identifier, Brand and MPN properties. These properties are highlighted in yellow but do not have red asterisk next the title.
![ExportFormProgress](/AdBOOST/images/exports/ExportFormProgress.png)

Some export properties can have only certain values supported by target network. It's up to you to choose feed property that fulfills these restrictions. Static values are validated automatically.
![ExportStaticFieldValid](/AdBOOST/images/exports/ExportStaticFieldValid.png)

AdBOOST allows you to map your item categories to values supported by export's target network. This feature is currently available for:

- Google Merchant Center [EN/CZ]
- Facebook [EN]
- Heureka [CZ/SK]
- Zbozi.cz [CZ]

 If you want to use this feature, you have to select property of your items that will be used as a mapping source.
![ExportCategoryMappingNotSelected](/AdBOOST/images/exports/ExportCategoryMappingNotSelected.png)

Afterwards, you can click "<i class="fa fa-wrench">&nbsp;</i> Map to {NETWORK} categories" button and you will see the dialog with values of selected property and inputs with fulltext search next to them. You can refine your searches until you find most suitable category supported by target network. Default value at the top of the modal will be used as a last option in case of missing feed property value, empty or unsuitable selected option.
![ExportCategoryMapping](/AdBOOST/images/exports/ExportCategoryMapping.png)

When you are satisfied with your category mapping, save the content of dialog. **If you close the dialog without saving, values will be lost**. Otherwise, you will notice that default value of attribute in main form has changed and green <i class="glyphicon glyphicon-ok">&nbsp;</i> icon has appeared in category property row to indicate that mapping is active.
![ExportCategoryMappingActive](/AdBOOST/images/exports/ExportCategoryMappingActive.png)

<script href="{{ '/assets/js/lightbox.min.js' | relative_url }}"></script>