---
layout: default
title:  "Banner Generator"
date:   2017-01-31 14:18:30 -0600
category: banner_generator
tags: [banner, generator, automated, template, display]
---

# Banner Generator

* TOC
{:toc}

## Getting started

Only pre-requisity of automated banners setup is to have at least one active data feed in AdBOOST. If you do not have one yet, please follow our [Feed setup guide](/AdBOOST{% post_url 2017-02-01-feed-setup %})

## Banners structure & usage

Banner feature of AdBOOST consists of following entities and tools:

- **Banner set** - item catalogs that hold consistent creatives for simmilar items. It's just a container for banner templates
- **Banner template** - specific creative type (e.g. green banner with badge and product image)
- **Banner editor** - tool for creation of banner templates in which you can specify text or image layers with remote content or content from your feed that will be transformed into banner ad
- **Banner ad** - every time, your feed is processed, every banner template, that uses this feed as a data source, will produce PNG image ad for every specific item from this feed

Each of these entities can be used differently:

- **Banner set** - can be assigned to <i class="network-icon adwords">&nbsp;</i> Google Display Network campaign
- **Banner template** - can be set as a product image for Facebook feed export
- **Banner ad** - can be downloaded as a PNG file or accessed via its persistent URL and therefore can be used in any display advertising network

## Banner set

In left context menu choose <i class="fa fa-image">&nbsp;</i> Banners > <i class="fa fa-object-group">&nbsp;</i> Banner sets.<br/>

{% include image_tag.html url="/AdBOOST/images/banners/LeftMenuBanners.png" alt="Left Menu Banners" style="height:200px;" %}

If you have not created any banner set yet, you will be greeted by welcome screen showing preview of banner setup steps and its example result.

{% include image_tag.html url="/AdBOOST/images/banners/BannersGuidedSetup.png" alt="Banners Guided Setup" style="" %}

If you have already created any banner sets, you will see them in listing and you will have the option to create new one by clicking <span class="btn btn-sm btn-primary"><i class="fa fa-plus">&nbsp;</i> Banner set</span> button

{% include image_tag.html url="/AdBOOST/images/banners/BannersListing.png" alt="Banners Listing" style="" %}

Click the <span class="btn btn-sm btn-primary"><i class="fa fa-plus">&nbsp;</i> Create your first banner set</span> button and you will be redirected to an empty form with one input for banner set name and another one with selection of your feeds from which you should choose one that will be used as a data source for a banner set. **Both fields are required and you won't be able to change the source feed later in the process**.

{% include image_tag.html url="/AdBOOST/images/banners/BannersEmptyForm.png" alt="Banners Empty Form" style="" %}

## Banner template

After you have filled in first two required properties of your banner set, it will be saved (but empty) and you will be presented with banner template create offer, which you can use in following ways:

- choose one of formats supported by your target network
- before selection, filter only formats with specific dimensions
- if none of prepared formats is suitable for your case, provide your custom dimensions

{% include image_tag.html url="/AdBOOST/images/banners/BannerTemplateGuidedSetup.png" alt="Banner Template Guided Setup" style="" %}

Some formats are suitable for more than one network and are therefore groupped into sets by this. When you choose your format and click the <span class="btn btn-sm btn-primary">Create</span> button, this selection will result into banner template with name in format: [UNI/AW/SKLIK/FB/INSTA/CUSTOM] - WIDTHxHEIGHT. This name can be later changed in banner editor.

## Banner editor

Banner template can be pre-viewed and modified in AdBOOST's banner editor. It's tool that consists of three main components:

1. **Layers pane** - orderable layers of two types (image/text) with type-specific options
2. **Template with placeholders** - placeholders that can be dragged and resized, which are showed in order that corresponds with order of their layers in layers pane. Image placeholders show informative preview of used image, text placeholders contain only text value
3. **Preview** - ads that are created in real-time to show you result of current template state processing

{% include image_tag.html url="/AdBOOST/images/banners/BannerEditor.png" alt="Banner Editor" style="" %}

## Layers

Layers pane contains list of template layers that can be added, removed and re-ordered. Colorpicker at the bottom of this pain sets template's background color. Each layer has it's type displayed as an icon and it's options that can be accessed by clicking on it.

### Text layer

Type of this layer is determined by value of selectbox at the top of the options pane.

{% include image_tag.html url="/AdBOOST/images/banners/TextLayer.png" alt="Text Layer" style="" %}

Content of the layer can be static, or you can use one of feed variables. You will see list of available feed variables if you hover with mouse pointer over the <i class="glyphicon glyphicon-info-sign">&nbsp;</i>icon

{% include image_tag.html url="/AdBOOST/images/banners/VariablesSuggestion.png" alt="Variables Suggestion" style="" %}

Every element of options pane has a tooltip, that will tell you what action it does (regardless of layer's type)

{% include image_tag.html url="/AdBOOST/images/banners/Tooltips.png" alt="Tooltips" style="" %}

We provide you with variety of Google fonts that you can use for your banners, or you can upload your custom font to preserve your identity accross channels.

{% include image_tag.html url="/AdBOOST/images/banners/FontSelection.png" alt="Font Selection" style="" %}

### Image layer

This layer can get it's content from three sources:

- Uploaded image
- Remote URL
- Feed variable

Either one of them will change layer's title and you will quickly know, what source is active. Source are chosen in order specified before. Simmilar as in case of text layer, you can see the list of available image variables from your feed by hovering over the <i class="glyphicon glyphicon-info-sign">&nbsp;</i>icon

{% include image_tag.html url="/AdBOOST/images/banners/ImageLayer.png" alt="Image Layer" style="" %}

In case of image layers, pay special attention to Fit to/Fill frame option. It can significantly change the resulting banner ad as you can see on examples below:

**Fill the frame image option**

{% include image_tag.html url="/AdBOOST/images/banners/FillFrame.png" alt="Fill Frame" style="" %}

**Fit to frame image option**

{% include image_tag.html url="/AdBOOST/images/banners/FitToFrame.png" alt="Fit To Frame" style="" %}

## Batch preview

If you click the <i class="glyphicon glyphicon-tasks">&nbsp;</i>icon at the top of the preview container, you will see batch preview of your currently modified banner template.

{% include image_tag.html url="/AdBOOST/images/banners/BatchPreview.png" alt="Batch Preview" style="" %}

This preview and also the single-banner preview generates only temporary banner ads, that won't be accessible outside of AdBOOST up to the point, when you submit banner editor changes.

## Control elements

All progress made in banner editor is only temporary if you do not save it. For the sake of optimization, banner editor has two submit buttons:

- **Save** - saves only the structure of banner template (layers, images, placeholders, ...) - good for saving of changes in the middle of the process
- **Save & Export** - saves the structure and triggers banner ads generating. Please use this button only if you really wish to generate ads

{% include image_tag.html url="/AdBOOST/images/banners/ControlElements.png" alt="ControlElements" style="" %}


