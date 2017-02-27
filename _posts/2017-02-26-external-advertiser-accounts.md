---
layout: default
title:  "External advertiser accounts"
date:   2017-02-26 12:53:14 -0600
category: "AdBOOST Core"
type: feature
trending: true
tags: [advertiser, adboost, accounts, setup, adwords, bing, bingads, sklik, seznam, heureka, facebook, analytics, merchant, center, shopping, zbozi, najnakup, srovname, business, data]
---

# External advertiser accounts

* TOC
{:toc}

## Introduction

AdBOOST as a platform can be connected to multiple advertising channels. Only requirement is that you already have your account set-up in target network. To make this process easier for you, we created this guide. Every part describes one network, how to manage your advertiser account for this network and where to find identifiers for AdBOOST.

## Google AdWords

This type of account is one of three types that require OAUTH verification. Warning icon at the top of the AdBOOST page will remain red until you connect your current AdBOOST e-mail to these advertising networks or accept these warnings as irrelevant (useful in case when your e-mail is not the one that is used as account owner in target network or when you do not want to manage advertising in all three networks)

{% include image_tag.html url="/images/advertiser_accounts/AdBoostOauths.png" alt="AdBoost Oauths" style="" %}

If you click to "<i class="fa fa-warning text-red"></i> AdWords not paired with your login", you will be redirected to Google's OAUTH page.

{% include image_tag.html url="/images/advertiser_accounts/AdBoostAdWordsOauth.png" alt="AdBoost AdWords Oauth" style="" %}

Here you can see what functionality will be accessible to AdBOOST. If you wish to continue, accept this form with click to "Allow" button. You will be redirected back to AdBOOST dashboard with notification about successful connection establishment. The number in red badge next to the warning icon will also change to reflect current number of connected network accounts.

Now that you have authentificated your current account with Google, you can connect it either to Google AdWords or [Google Analytics](#google-analytics). Let's continue with AdWords. Visit AdBOOST's product campaigns dashboard.

{% include image_tag.html url="/images/advertiser_accounts/LeftMenuDashboard.png" alt="Left Menu Dashboard" style="height:200px;" %}

Here you can see three tiles with titles of PPC advertising networks and smiley face describing status of their connection.

{% include image_tag.html url="/images/advertiser_accounts/AdBoostDashboardConnections.png" alt="AdBoost Dashboard Connections" style="" %}

Proceed with click to "<i class="network-icon aw"></i> AdWords". You will be presented with dialog that contains the connection form.

{% include image_tag.html url="/images/advertiser_accounts/AdBoostAdWordsConnect.png" alt="AdBoost AdWords Connect" style="" %}

**AdWords Account** is a selectbox, where you can choose one of emails that has been connected to your current AdBoost account (you probably want to choose your current email, that you have verified in previous step)

**AdWords ID** is an identifier of your AdWords account. If you do not have one yet, you can create it at: <a href="https://adwords.google.com/" target="_blank">adwords.google.com</a> Afterwards, you can find your AdWords ID in the part of AdWords interface displayed on the screen below.

{% include image_tag.html url="/images/advertiser_accounts/AdWords.png" alt="AdWords" style="" %}

Click the "Verify" button in the dialog and AdWords tile will change status after successful account pairing.

{% include image_tag.html url="/images/advertiser_accounts/AdBoostAdWordsConnected.png" alt="AdBoost AdWords Connected" style="height:200px;" %}

## Sklik.cz

AdBOOST can be connected to Sklik.cz with combination of e-mail and password (since Sklik currently does not provide OAUTH authentification). If you visit AdBOOST's product campaigns dashboard.

{% include image_tag.html url="/images/advertiser_accounts/LeftMenuDashboard.png" alt="Left Menu Dashboard" style="height:200px;" %}

You can see three tiles with titles of PPC advertising networks and smiley face describing status of their connection.

{% include image_tag.html url="/images/advertiser_accounts/AdBoostDashboardConnections.png" alt="AdBoost Dashboard Connections" style="" %}

Proceed with click to "<i class="network-icon sklik"></i> Sklik". You will be presented with dialog that contains the connection form.

{% include image_tag.html url="/images/advertiser_accounts/AdBoostSklikConnect.png" alt="AdBoost Sklik Connect" style="" %}

Sklik Email and Password is the combination that you use to access any of your Sklik accounts.

{% include image_tag.html url="/images/advertiser_accounts/SklikAccount.png" alt="Sklik Account" style="" %}

## Bing Ads

This type of account is one of three types that require OAUTH verification. Warning icon at the top of the AdBOOST page will remain red until you connect your current AdBOOST e-mail to these advertising networks or accept these warnings as irrelevant (useful in case when your e-mail is not the one that is used as account owner in target network or when you do not want to manage advertising in all three networks)

{% include image_tag.html url="/images/advertiser_accounts/AdBoostOauths.png" alt="AdBoost Oauths" style="" %}

If you click to "<i class="fa fa-warning text-red"></i> Bing Ads not paired with your login", you will be redirected to Microsoft's OAUTH page. Successful authentification will redirect you back to AdBOOST dashboard with notification about successful connection establishment. The number in red badge next to the warning icon will also change to reflect current number of connected network accounts.

Now that you have authentificated your current account with Microsoft, you can connect it to Bing Ads. Visit AdBOOST's product campaigns dashboard.

{% include image_tag.html url="/images/advertiser_accounts/LeftMenuDashboard.png" alt="Left Menu Dashboard" style="height:200px;" %}

Here you can see three tiles with titles of PPC advertising networks and smiley face describing status of their connection.

{% include image_tag.html url="/images/advertiser_accounts/AdBoostDashboardConnections.png" alt="AdBoost Dashboard Connections" style="" %}

Proceed with click to "<i class="network-icon bing"></i> Bing Ads". You will be presented with dialog that contains the connection form.

{% include image_tag.html url="/images/advertiser_accounts/AdBoostBingAdsConnect.png" alt="AdBoost BingAds Connect" style="" %}

All three required identifiers can be found in the "Accounts & Billing" part of your Bing Ads account. To access Bing Ads, you first have to posess the Microsoft account. Afterwars, you can navigate to: <a href="https://ui.bingads.microsoft.com" target="_blank">bingads.microsoft.com/</a> If do not already have a Bing Ads account, create one by providing you Microsoft account info.

{% include image_tag.html url="/images/advertiser_accounts/BingAdsAccountCreate.png" alt="Bing Ads Account Create" style="" %}

Afterwards, you can specify whether you wish to import some of your existing PPC campaigns from AdWords or you want to start from scratch.

{% include image_tag.html url="/images/advertiser_accounts/BingAdsCampaignsSettings.png" alt="Bing Ads Campaigns Settings" style="" %}

When you successfuly setup your Bing Ads account, you will be redirected to your Ads Dashboard. Navigate to "Accounts & Billing" part.

{% include image_tag.html url="/images/advertiser_accounts/BingAdsDashboard.png" alt="Bing Ads Dashboard" style="" %}

This is the part where you can find all credentials that are needed to connect AdBoost to your Bing Ads account.

{% include image_tag.html url="/images/advertiser_accounts/BingAdsCredentials.png" alt="Bing Ads Credentials" style="" %}

## Facebook Ads

## Google Analytics

## Heureka

## Google Merchant Center

## Zboží.cz

## Najnákup.sk

## Srovnáme.cz

## Google Business Data

