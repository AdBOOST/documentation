---
layout: default
title:  "External Advertiser Accounts"
date:   2017-02-26 12:53:14 -0600
category: "AdBOOST Core"
type: feature
trending: true
tags: [advertiser, adboost, accounts, setup, adwords, bing, bingads, sklik, seznam, heureka, facebook, analytics, merchant, center, shopping, zbozi, najnakup, srovname, business, data, remarketing]
---

# External Advertiser Accounts

* TOC
{:toc}

## Introduction

AdBOOST as a platform can be connected to multiple advertising channels. Only requirement is that you already have your account set-up in target network. To make this process easier for you, we created this guide. Every part describes one network, how to manage your advertiser account for this network and where to find identifiers for AdBOOST.

## Google AdWords

This type of account is one of three types that require OAUTH verification. Warning icon at the top of the AdBOOST page will remain red until you connect your current AdBOOST e-mail to these advertising networks or accept these warnings as irrelevant (useful in case when your e-mail is not the one that is used as account owner in target network or when you do not want to manage advertising in all three networks)

{% include image_tag.html url="/images/advertiser_accounts/AdBoostOauths.png" alt="AdBoost Oauths" style="" %}

Another place, where you can create Google OAUTH connections for your account at any time is product campaigns dashboard. Here you can see three tiles with titles of PPC advertising networks and smiley face describing status of their connection.

{% include image_tag.html url="/images/advertiser_accounts/AdBoostDashboardConnections.png" alt="AdBoost Dashboard Connections" style="" %}

If you click to "<i class="fa fa-warning text-red"></i> AdWords not paired with your login" or if you use the <i class="fa fa-plus"></i> button inside the dialog invoked by click to the AdWords tile (see [AdWords Account](#adwordsOauth)) on the product campaigns dashboard, you will be redirected to Google's OAUTH page.

{% include image_tag.html url="/images/advertiser_accounts/AdBoostAdWordsOauth.png" alt="AdBoost AdWords Oauth" style="" %}

Here you can see what functionality will be accessible to AdBOOST. If you wish to continue, accept this form with click to "Allow" button. You will be redirected back to AdBOOST dashboard with notification about successful connection establishment. The number in red badge next to the warning icon will also change to reflect current number of connected network accounts.

Now that you have authenticated your current account with Google, you can connect it either to Google AdWords or [Google Analytics](#google-analytics). Let's continue with AdWords. Return to AdBOOST's product campaigns dashboard.

{% include image_tag.html url="/images/advertiser_accounts/LeftMenuDashboard.png" alt="Left Menu Dashboard" style="height:250px;" %}

Navigate towards three tiles with titles of PPC advertising networks and smiley face describing status of their connection.

{% include image_tag.html url="/images/advertiser_accounts/AdBoostDashboardConnections.png" alt="AdBoost Dashboard Connections" style="" %}

Proceed with click to "<i class="network-icon aw"></i> AdWords". <a name="adwordsOauth"></a> You will be presented with dialog that contains the connection form.

{% include image_tag.html url="/images/advertiser_accounts/AdBoostAdWordsConnect.png" alt="AdBoost AdWords Connect" style="height:300px;" %}

**AdWords Account** is a selectbox, where you can choose one of emails that have been connected to your current AdBoost account. You probably want to choose your current email, that you might have verified in the previous steps. If you have not, you can still make so by clicking the <i class="fa fa-plus"></i> icon. This will connect your current e-mail (the one you used to log in) with Google OAUTH.

**AdWords ID** is an identifier of your AdWords account. If you do not have one yet, you can create it at: <a href="https://adwords.google.com/" target="_blank">adwords.google.com</a> Afterwards, you can find your AdWords ID in the part of AdWords interface displayed on the screen below.

{% include image_tag.html url="/images/advertiser_accounts/AdWords.png" alt="AdWords" style="" %}

Click the "Verify" button in the dialog and AdWords tile will change status after successful account pairing.

{% include image_tag.html url="/images/advertiser_accounts/AdBoostAdWordsConnected.png" alt="AdBoost AdWords Connected" style="height:250px;" %}

## Sklik.cz

AdBOOST can be connected to Sklik.cz with combination of e-mail and password (since Sklik currently does not provide OAUTH authentification). If you visit AdBOOST's product campaigns dashboard.

{% include image_tag.html url="/images/advertiser_accounts/LeftMenuDashboard.png" alt="Left Menu Dashboard" style="height:250px;" %}

You can see three tiles with titles of PPC advertising networks and smiley face describing status of their connection.

{% include image_tag.html url="/images/advertiser_accounts/AdBoostDashboardConnections.png" alt="AdBoost Dashboard Connections" style="" %}

Proceed with click to "<i class="network-icon sklik"></i> Sklik". You will be presented with dialog that contains the connection form.

{% include image_tag.html url="/images/advertiser_accounts/AdBoostSklikConnect.png" alt="AdBoost Sklik Connect" style="height:300px;" %}

Sklik Email and Password is the combination that you use to access any of your Sklik accounts.

{% include image_tag.html url="/images/advertiser_accounts/SklikAccount.png" alt="Sklik Account" style="" %}

## Bing Ads

This type of account is one of three types that require OAUTH verification. Warning icon at the top of the AdBOOST page will remain red until you connect your current AdBOOST e-mail to these advertising networks or accept these warnings as irrelevant (useful in case when your e-mail is not the one that is used as account owner in target network or when you do not want to manage advertising in all three networks)

{% include image_tag.html url="/images/advertiser_accounts/AdBoostOauths.png" alt="AdBoost Oauths" style="" %}

If you click to "<i class="fa fa-warning text-red"></i> Bing Ads not paired with your login", you will be redirected to Microsoft's OAUTH page. Successful authentification will redirect you back to AdBOOST dashboard with notification about successful connection establishment. The number in red badge next to the warning icon will also change to reflect current number of connected network accounts.

Now that you have authentificated your current account with Microsoft, you can connect it to Bing Ads. Visit AdBOOST's product campaigns dashboard.

{% include image_tag.html url="/images/advertiser_accounts/LeftMenuDashboard.png" alt="Left Menu Dashboard" style="height:250px;" %}

Here you can see three tiles with titles of PPC advertising networks and smiley face describing status of their connection.

{% include image_tag.html url="/images/advertiser_accounts/AdBoostDashboardConnections.png" alt="AdBoost Dashboard Connections" style="" %}

Proceed with click to "<i class="network-icon bing"></i> Bing Ads". You will be presented with dialog that contains the connection form.

{% include image_tag.html url="/images/advertiser_accounts/AdBoostBingAdsConnect.png" alt="AdBoost BingAds Connect" style="height:300px;" %}

All three required identifiers can be found in the "Accounts & Billing" part of your Bing Ads account. To access Bing Ads, you first have to posess the Microsoft account. Afterwars, you can navigate to: <a href="https://ui.bingads.microsoft.com" target="_blank">bingads.microsoft.com/</a> If do not already have a Bing Ads account, create one by providing you Microsoft account info.

{% include image_tag.html url="/images/advertiser_accounts/BingAdsAccountCreate.png" alt="Bing Ads Account Create" style="" %}

Afterwards, you can specify whether you wish to import some of your existing PPC campaigns from AdWords or you want to start from scratch.

{% include image_tag.html url="/images/advertiser_accounts/BingAdsCampaignsSettings.png" alt="Bing Ads Campaigns Settings" style="" %}

When you successfuly setup your Bing Ads account, you will be redirected to your Ads Dashboard. Navigate to "Accounts & Billing" part.

{% include image_tag.html url="/images/advertiser_accounts/BingAdsDashboard.png" alt="Bing Ads Dashboard" style="" %}

This is the part where you can find all credentials that are needed to connect AdBoost to your Bing Ads account.

{% include image_tag.html url="/images/advertiser_accounts/BingAdsCredentials.png" alt="Bing Ads Credentials" style="" %}

## Facebook Ads

### As a data source

This type of account is one of three types that require OAUTH verification. Warning icon at the top of the AdBOOST page will remain red until you connect your current AdBOOST e-mail to these advertising networks or accept these warnings as irrelevant (useful in case when your e-mail is not the one that is used as account owner in target network or when you do not want to manage advertising in all three networks)

{% include image_tag.html url="/images/advertiser_accounts/AdBoostOauths.png" alt="AdBoost Oauths" style="" %}

Another place, where you can create Facebook OAUTH connections for your account at any time is feed management dashboard. Here you can see one tile with Facebook icon and smiley face describing status of your connection with this network.

{% include image_tag.html url="/images/advertiser_accounts/FeedDashboardConnections.png" alt="Feed Dashboard Connections" style="" %}

If you click to "<i class="fa fa-warning text-red"></i> Facebook not paired with your login" or if you use the <i class="fa fa-plus"></i> button inside the dialog invoked by click to the Facebook tile (see [Facebook Account](#facebookOauth)) on the feed management dashboard, you will be redirected to Facebook's OAUTH page.

{% include image_tag.html url="/images/advertiser_accounts/AdBoostFacebookOauth.png" alt="AdBoost Facebook Oauth" style="" %}

If you submit this form, you will only give AdBOOST access to you public profile and e-mail address. Access to your Facebook Ads account will be requested only after this step.

{% include image_tag.html url="/images/advertiser_accounts/AdBoostFacebookAds.png" alt="AdBoost Facebook Ads" style="" %}

This connection can be utilized in process of your Facebook advertising performance monitoring with our [Monitoring Tool]({% post_url 2017-02-06-monitoring-tool %}). It provides interface for external channels setup. Here you will need your account identifier to fetch your Facebook Ads account stats.

{% include image_tag.html url="/images/MonitoringAccounts.png" alt="Monitoring Accounts" style="" %}

This number can be obtained from your Facebook Ads interface. This interface is accessed by selecting a "Create Adverts" option in your Facebook account.

{% include image_tag.html url="/images/advertiser_accounts/FacebookDashboard.png" alt="Facebook Dashboard" style="" %}

Desired <a name="facebookCreateAds"></a> Facebook Ads account number can then be found in the selectbox with your accessible accounts.

{% include image_tag.html url="/images/advertiser_accounts/FacebookCredentials.png" alt="Facebook Credentials" style="" %}

As mentioned before, another way how you can connect to Facebook at any time is to click the Facebook tile with smiley face on feed management dashboard.

{% include image_tag.html url="/images/advertiser_accounts/FeedDashboardConnections.png" alt="Feed Dashboard Connections" style="" %}

You will be presented with dialog that contains the connection form. <a name="facebookOauth"></a>

{% include image_tag.html url="/images/advertiser_accounts/AdBoostFacebookConnect.png" alt="AdBoost AdWords Connect" style="height:300px;" %}

**Facebook Account Email** is a selectbox, where you can choose one of emails that have been connected to your current AdBoost account. You probably want to choose your current email, that you might have verified in the previous steps. If you have not, you can still make so by clicking the <i class="fa fa-plus"></i> icon. This will connect your current e-mail (the one you used to log in) with Facebook OAUTH.

**Facebook ID** is an identifier of your Facebook account, whose location was described two steps ago.

### As an export target

Second way how to use AdBOOST in combination with Facebook is to create product catalogues. These can be found in your advertiser account that has been previously mentioned in [Facebook Create-Ads](#facebookCreateAds). Quickest way how to find this part of Facebook interface is to use searchbar at the top of your advertiser account.

{% include image_tag.html url="/images/advertiser_accounts/FacebookCataloguesSearch.png" alt="Facebook Catalogues Search" style="" %}

Afterwards, continue with clicks to **Product Feeds** tab and **<i class="fa fa-plus"></i> Add Product Feed** button

{% include image_tag.html url="/images/advertiser_accounts/FacebookAddFeed.png" alt="Facebook Add Feed" style="" %}

Name your feed and keep the **Scheduled recurring uploads** option selected. Contiue with click to the **Next** button

{% include image_tag.html url="/images/advertiser_accounts/FacebookFeedCreate.png" alt="Facebook Feed Create" style="" %}

This is when AdBOOST comes into the play. Feed URL that has to be set-up in the next step can be obtained from any one of your Facebook feed exports in your AdBOOST account. In Facebook:

{% include image_tag.html url="/images/advertiser_accounts/FacebookFeedSave.png" alt="Facebook Feed Save" style="" %}

And in AdBOOST:

{% include image_tag.html url="/images/advertiser_accounts/FacebookExportURL.png" alt="Facebook Export URL" style="" %}

Result of this procedure is your own product catalog that is ready to be released and shown in form of ads to your customers.

{% include image_tag.html url="/images/advertiser_accounts/FacebookProductCatalog.png" alt="Facebook Product Catalog" style="" %}

## Google Analytics

This type of account can be utilized in process of your Google Analytics site monitoring with our [Monitoring Tool]({% post_url 2017-02-06-monitoring-tool %}). It is interesting mostly for cross-validation of statistics provided by other advertising networks. Monitoring tool provides interface for external channels setup. Here you will need your account identifier to fetch your Analytics account stats.

{% include image_tag.html url="/images/MonitoringAccounts.png" alt="Monitoring Accounts" style="" %}

This number can be obtained from your <a href="https://analytics.google.com/" target="_blank">Google Analytics interface</a>.

{% include image_tag.html url="/images/advertiser_accounts/AnalyticsCredentials.png" alt="Analytics Credentials" style="" %}

After it has been provided into form, you will be presented with another two fields:

1. **Property ID** - segment of your analytics account e.g. language versions of same website
2. **View ID** - event set within account segment defined by you. Default value equals to "All Web Site Data"

{% include image_tag.html url="/images/advertiser_accounts/AnalyticsProps.png" alt="Analytics Props" style="" %}

These can be found after the click to the selectbox at the top left corner of Google Analytics interface.

{% include image_tag.html url="/images/advertiser_accounts/AnalyticsTriplet.png" alt="Analytics Triplet" style="" %}

## Heureka

This type of account can be utilized either as a source in the process of your Heureka account monitoring with our [Monitoring Tool]({% post_url 2017-02-06-monitoring-tool %}) or as a target for your [Heureka Feed Export]({% post_url 2017-01-30-feed-exports %}).

### As a data source

Monitoring tool provides interface for external channels setup. Here you will need your account identifier to fetch your Heureka account stats. In this case account identifier is URL address of your daily conversion report.

{% include image_tag.html url="/images/MonitoringAccounts.png" alt="Monitoring Accounts" style="" %}

This URL can be obtained from Heureka interface, specifically from part "Prehľad vašich obchodov > Meranie konverzií"

{% include image_tag.html url="/images/advertiser_accounts/HeurekaReport.png" alt="Heureka Report" style="" %}

### As an export target

In this case you want AdBOOST to keep your Heureka feed up-to-date, with correct categories and CPC. You should navigate to "Prehľad vašich obchodov > Prehľad" part of Heureka interface. and choose the option "Upraviť obchod".

{% include image_tag.html url="/images/advertiser_accounts/HeurekaZone.png" alt="Heureka Zone" style="" %}

Here you should be able to change "Url XML Importu"

{% include image_tag.html url="/images/advertiser_accounts/HeurekaURL.png" alt="Heureka URL" style="" %}

This URL can be obtained from the top of the Heureka Feed Export form or from the Exports listing.

{% include image_tag.html url="/images/advertiser_accounts/AdBoostHeurekaURL.png" alt="Adboost Heureka URL" style="" %}

## Google Merchant Center

This type of account utilizes our [Exports for external networks]({% post_url 2017-01-30-feed-exports %}#export-status). If you export your feed data to AdBOOST URL with schema following rules of Google Merchant Center, you can insert this URL into MCC interface and quickly get your products to be shown in search results and in Google Shopping. To achieve this, navigate to <a href="http://merchants.google.com/" target="_blank">merchants.google.com</a> and to the "Products" part of the dashboard.

{% include image_tag.html url="/images/advertiser_accounts/MerchantCenterDashboard.png" alt="Merchant Center Dashboard" style="" %}

Click the big <i class="fa fa-plus"></i> button to add your Feed. Name it according to your domain and its purpose.

{% include image_tag.html url="/images/advertiser_accounts/MerchantCenterFeedAdd.png" alt="Merchant Center Feed Add" style="" %}

Assign a correct type to it. Since the AdBOOST will update your products on static URL every time when change occurs in your feed, you should point your MCC feed to this URL. Therefore select "Schedule fetch" option and click "Continue".

{% include image_tag.html url="/images/advertiser_accounts/MerchantCenterFeedFetch.png" alt="Merchant Center Feed Fetch" style="" %}

Last part of this form is where you should insert URL of your MCC export.

{% include image_tag.html url="/images/advertiser_accounts/MerchantCenterFeedSave.png" alt="Merchant Center Feed Save" style="" %}

This URL can be found at the top of every [Export form]({% post_url 2017-01-30-feed-exports %}#export-status)

{% include image_tag.html url="/images/advertiser_accounts/ExportURL.png" alt="Export URL" style="" %}

and in the actions column of export listing.

{% include image_tag.html url="/images/advertiser_accounts/MccExportListingURL.png" alt="Mcc Export Listing URL" style="" %}

## Google Business Data

This is only one part of Google AdWords interface, that is designed to provide functionallity related to dynamic display ad data - **remarketing**. You can find it in the left context menu under Shared library. This data combines Google's records of your audience with descriptions of your products obtained from your feed in CSV. To setup your feed, follow steps on the screen below.

{% include image_tag.html url="/images/advertiser_accounts/BusinessData.png" alt="Business Data" style="" %}

When you are done, you can upload CSV file with description of your products

{% include image_tag.html url="/images/advertiser_accounts/BusinessDataFeed.png" alt="Business Data Feed" style="" %}

this file can be downloaded from AdBOOST's feed exports after you have created export of this type following the [Feed Exports guide]({% post_url 2017-01-30-feed-exports %}).

{% include image_tag.html url="/images/advertiser_accounts/BusinessDataURL.png" alt="Business Data URL" style="" %}

## Zboží.cz

This type of account utilizes our [Exports for external networks]({% post_url 2017-01-30-feed-exports %}#export-status). If you export your feed data to AdBOOST URL with schema following rules of Zboží.cz, you can insert this URL into Zboží.cz interface and quickly get your products to be shown in product comparisons. To achieve this, navigate to <a href="https://www.zbozi.cz/" target="_blank">www.zbozi.cz</a> and to the "Administrace" part of the page.

{% include image_tag.html url="/images/advertiser_accounts/ZboziLogin.png" alt="Zbozi Login" style="" %}

You should be able to find list of your products feeds where you can manage their URLs after click to "Editace URL feedu"

{% include image_tag.html url="/images/advertiser_accounts/ZboziFeeds.png" alt="Zbozi Feeds" style="" %}

After that you should be able to specify URL of your AdBOOST export and request its periodic processing.

{% include image_tag.html url="/images/advertiser_accounts/ZboziURL.png" alt="Zbozi URL" style="" %}

This URL can be obtained from the top of the Zboží.cz Feed Export form or from the Exports listing.

{% include image_tag.html url="/images/advertiser_accounts/AdBoostZboziURL.png" alt="Adboost Zbozi URL" style="" %}

