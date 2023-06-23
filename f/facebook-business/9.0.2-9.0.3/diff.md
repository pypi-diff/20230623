# Comparing `tmp/facebook_business-9.0.2.tar.gz` & `tmp/facebook_business-9.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facebook_business-9.0.2.tar", last modified: Thu Jan 14 01:49:23 2021, max compression
+gzip compressed data, was "facebook_business-9.0.3.tar", last modified: Tue Feb 16 23:49:27 2021, max compression
```

## Comparing `facebook_business-9.0.2.tar` & `facebook_business-9.0.3.tar`

### file list

```diff
@@ -1,670 +1,672 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-14 01:49:23.256527 facebook_business-9.0.2/
--rw-r--r--   0 runner    (1001) docker     (116)     3352 2021-01-14 01:49:10.000000 facebook_business-9.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (116)      249 2021-01-14 01:49:10.000000 facebook_business-9.0.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (116)     1895 2021-01-14 01:49:10.000000 facebook_business-9.0.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (116)     1045 2021-01-14 01:49:10.000000 facebook_business-9.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1166 2021-01-14 01:49:10.000000 facebook_business-9.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)    21400 2021-01-14 01:49:23.252527 facebook_business-9.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    17278 2021-01-14 01:49:10.000000 facebook_business-9.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-14 01:49:23.192526 facebook_business-9.0.2/examples/
--rw-r--r--   0 runner    (1001) docker     (116)     1413 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountActivityNode.py
--rw-r--r--   0 runner    (1001) docker     (116)     1476 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdCreativesEdge.py
--rw-r--r--   0 runner    (1001) docker     (116)     1544 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdCreativesPost.py
--rw-r--r--   0 runner    (1001) docker     (116)     1650 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdCreativesPost2CreateAdCreativeLinkAd.py
--rw-r--r--   0 runner    (1001) docker     (116)     1703 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdCreativesPost2CreateLinkAdCallToActionAppInstall.py
--rw-r--r--   0 runner    (1001) docker     (116)     1671 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdCreativesPost2CreateLinkAdImageCrop.py
--rw-r--r--   0 runner    (1001) docker     (116)     1898 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdCreativesPost2CreateMAIDPA.py
--rw-r--r--   0 runner    (1001) docker     (116)     1712 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdCreativesPost2CreateVideoLeadAd.py
--rw-r--r--   0 runner    (1001) docker     (116)     1673 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdCreativesPost2CreateVideoPageLikeAd.py
--rw-r--r--   0 runner    (1001) docker     (116)     1715 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdCreativesPost3CreateAdCreativePageLike.py
--rw-r--r--   0 runner    (1001) docker     (116)     1976 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdCreativesPost3CreateAssetFeedSpec.py
--rw-r--r--   0 runner    (1001) docker     (116)     2363 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdCreativesPost3CreateCarouselCallToActionAppInstall.py
--rw-r--r--   0 runner    (1001) docker     (116)     2290 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdCreativesPost3CreateDynamicAdCustomization.py
--rw-r--r--   0 runner    (1001) docker     (116)     1510 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdCreativesPostCreateAdCreative.py
--rw-r--r--   0 runner    (1001) docker     (116)     1673 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdCreativesPostCreateAdCreativeCanvas.py
--rw-r--r--   0 runner    (1001) docker     (116)     1972 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdCreativesPostCreateAdCreativeCustomizationCanvasDV.py
--rw-r--r--   0 runner    (1001) docker     (116)     1981 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdCreativesPostCreateAdCreativeCustomizationCanvasImage.py
--rw-r--r--   0 runner    (1001) docker     (116)     2043 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdCreativesPostCreateAdCreativeCustomizationCanvasVideo.py
--rw-r--r--   0 runner    (1001) docker     (116)     1950 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdSetsPost2CreateMAIA.py
--rw-r--r--   0 runner    (1001) docker     (116)     1945 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdSetsPostAdSetCreateCpa.py
--rw-r--r--   0 runner    (1001) docker     (116)     2002 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdSetsPostAdSetCreateCpaAppEvents.py
--rw-r--r--   0 runner    (1001) docker     (116)     1833 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdSetsPostBehaviorTargeting.py
--rw-r--r--   0 runner    (1001) docker     (116)     1941 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdSetsPostBidMultiplier.py
--rw-r--r--   0 runner    (1001) docker     (116)     2220 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdSetsPostCreateAdSet.py
--rw-r--r--   0 runner    (1001) docker     (116)     1809 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdSetsPostCreateAudienceNetwork.py
--rw-r--r--   0 runner    (1001) docker     (116)     1840 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdSetsPostDailyBudget20.py
--rw-r--r--   0 runner    (1001) docker     (116)     2194 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdSetsPostDemographicTargeting.py
--rw-r--r--   0 runner    (1001) docker     (116)     2092 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdSetsPostInterestTargeting.py
--rw-r--r--   0 runner    (1001) docker     (116)     1898 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdSetsPostLifetimeBudget200Duration10Days.py
--rw-r--r--   0 runner    (1001) docker     (116)     1941 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdSetsPostOfferClaim.py
--rw-r--r--   0 runner    (1001) docker     (116)     2164 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdSetsPostOptimizePostEngagement.py
--rw-r--r--   0 runner    (1001) docker     (116)     1792 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdSetsPostPageLikes.py
--rw-r--r--   0 runner    (1001) docker     (116)     1798 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdSetsPostPlacementTargeting.py
--rw-r--r--   0 runner    (1001) docker     (116)     1846 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdSetsPostReach.py
--rw-r--r--   0 runner    (1001) docker     (116)     1486 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdVideosPost.py
--rw-r--r--   0 runner    (1001) docker     (116)     1397 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdsPixelEdgeGetPixelCode.py
--rw-r--r--   0 runner    (1001) docker     (116)     1488 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdsPixelsPost.py
--rw-r--r--   0 runner    (1001) docker     (116)     1559 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdsPost.py
--rw-r--r--   0 runner    (1001) docker     (116)     1601 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdsPostAdsRedownload.py
--rw-r--r--   0 runner    (1001) docker     (116)     1724 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdsPostOfferClaim.py
--rw-r--r--   0 runner    (1001) docker     (116)     1656 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountAdsPostTrackingPostEngagement.py
--rw-r--r--   0 runner    (1001) docker     (116)     1527 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountCampaignsEdge.py
--rw-r--r--   0 runner    (1001) docker     (116)     1578 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountCampaignsPostConversions.py
--rw-r--r--   0 runner    (1001) docker     (116)     1585 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountCampaignsPostEventResponses.py
--rw-r--r--   0 runner    (1001) docker     (116)     1586 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountCampaignsPostLeadGen.py
--rw-r--r--   0 runner    (1001) docker     (116)     1569 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountCampaignsPostLinkClicks.py
--rw-r--r--   0 runner    (1001) docker     (116)     1569 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountCampaignsPostLocalAwareness.py
--rw-r--r--   0 runner    (1001) docker     (116)     1587 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountCampaignsPostMAIA.py
--rw-r--r--   0 runner    (1001) docker     (116)     1605 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountCampaignsPostMAIDPA.py
--rw-r--r--   0 runner    (1001) docker     (116)     1583 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountCampaignsPostOfferClaims.py
--rw-r--r--   0 runner    (1001) docker     (116)     1574 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountCampaignsPostPageLikes.py
--rw-r--r--   0 runner    (1001) docker     (116)     1579 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountCampaignsPostPostEngagement.py
--rw-r--r--   0 runner    (1001) docker     (116)     1626 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountCampaignsPostStoreCampaign.py
--rw-r--r--   0 runner    (1001) docker     (116)     1578 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountCampaignsPostVideoViews.py
--rw-r--r--   0 runner    (1001) docker     (116)     1486 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountCustomAudiencesEdge.py
--rw-r--r--   0 runner    (1001) docker     (116)     1508 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountCustomAudiencesEdgeDataSourceSubtype.py
--rw-r--r--   0 runner    (1001) docker     (116)     1642 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountCustomAudiencesPostCreateCustomAudience.py
--rw-r--r--   0 runner    (1001) docker     (116)     1703 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountCustomAudiencesPostDynamicEventValueBasedLookalikeCustomAudience.py
--rw-r--r--   0 runner    (1001) docker     (116)     1675 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountCustomAudiencesPostDynamicValueBasedLookalikeCustomAudience.py
--rw-r--r--   0 runner    (1001) docker     (116)     1775 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountCustomAudiencesPostPlatformCustomAudienceMACARule.py
--rw-r--r--   0 runner    (1001) docker     (116)     2001 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountCustomAudiencesPostPlatformECAExclusions.py
--rw-r--r--   0 runner    (1001) docker     (116)     1835 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountCustomAudiencesPostPlatformECAMultiFilters.py
--rw-r--r--   0 runner    (1001) docker     (116)     1811 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountCustomAudiencesPostPlatformECAMultiPages.py
--rw-r--r--   0 runner    (1001) docker     (116)     1778 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountCustomAudiencesPostPlatformEngagementCustomAudience.py
--rw-r--r--   0 runner    (1001) docker     (116)     1772 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountCustomAudiencesPostPlatformWebsiteCustomAudience.py
--rw-r--r--   0 runner    (1001) docker     (116)     1620 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountCustomAudiencesPostValueBasedCustomAudience.py
--rw-r--r--   0 runner    (1001) docker     (116)     1670 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountCustomAudiencesPostValueBasedLookalikeCustomAudience.py
--rw-r--r--   0 runner    (1001) docker     (116)     1532 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountGeneratePreviewsEdge.py
--rw-r--r--   0 runner    (1001) docker     (116)     1564 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountGeneratePreviewsEdgeDesktopWithStoryId.py
--rw-r--r--   0 runner    (1001) docker     (116)     1776 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountGeneratePreviewsEdgeInstagramStandards.py
--rw-r--r--   0 runner    (1001) docker     (116)     1743 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountGeneratePreviewsEdgeMaiaWithObjectStorySpec.py
--rw-r--r--   0 runner    (1001) docker     (116)     1401 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountNode.py
--rw-r--r--   0 runner    (1001) docker     (116)     1775 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountProductAudiencesPostIphoneViewNoPurchase.py
--rw-r--r--   0 runner    (1001) docker     (116)     1786 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountProductAudiencesPostNoPurchase.py
--rw-r--r--   0 runner    (1001) docker     (116)     1578 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdAccountReachEstimate.py
--rw-r--r--   0 runner    (1001) docker     (116)     1395 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdCampaignActivityNode.py
--rw-r--r--   0 runner    (1001) docker     (116)     1404 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdCampaignGroupActivityNode.py
--rw-r--r--   0 runner    (1001) docker     (116)     1449 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdCampaignGroupAdsEdge.py
--rw-r--r--   0 runner    (1001) docker     (116)     1485 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdCampaignGroupAdsEdgeAdgroupsWithStatusArchived.py
--rw-r--r--   0 runner    (1001) docker     (116)     1528 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdCampaignGroupAdsetsEdge.py
--rw-r--r--   0 runner    (1001) docker     (116)     1395 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdCampaignNode.py
--rw-r--r--   0 runner    (1001) docker     (116)     1547 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdCampaignPost.py
--rw-r--r--   0 runner    (1001) docker     (116)     1558 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdCampaignPostAdsetUpdateCpa.py
--rw-r--r--   0 runner    (1001) docker     (116)     1517 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdCreativeCreativeInsightsEdge.py
--rw-r--r--   0 runner    (1001) docker     (116)     1416 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdCreativeNode.py
--rw-r--r--   0 runner    (1001) docker     (116)     1426 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdCreativeNodeRead.py
--rw-r--r--   0 runner    (1001) docker     (116)     1424 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdCreativeNodeReadInstagramPermalinkUrl.py
--rw-r--r--   0 runner    (1001) docker     (116)     1547 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdCreativePreviewsEdge.py
--rw-r--r--   0 runner    (1001) docker     (116)     1504 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdCreativePreviewsEdgePreview.py
--rw-r--r--   0 runner    (1001) docker     (116)     1547 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdCreativePreviewsEdgePreviewDynamicAds.py
--rw-r--r--   0 runner    (1001) docker     (116)     1611 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdCreativePreviewsEdgePreviewDynamicAdsWithCustomizations.py
--rw-r--r--   0 runner    (1001) docker     (116)     1425 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdgroupActivityNode.py
--rw-r--r--   0 runner    (1001) docker     (116)     1424 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdgroupLeadsEdgeAdgroupLeads.py
--rw-r--r--   0 runner    (1001) docker     (116)     1462 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdgroupLeadsEdgeAdgroupLeadsDPA.py
--rw-r--r--   0 runner    (1001) docker     (116)     1512 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdgroupLeadsEdgeAdgroupLeadsFiltered.py
--rw-r--r--   0 runner    (1001) docker     (116)     1393 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdgroupPost.py
--rw-r--r--   0 runner    (1001) docker     (116)     1400 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdgroupPostUpdateStatus.py
--rw-r--r--   0 runner    (1001) docker     (116)     1502 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdsInsightsEdgeAdCampaignInsights.py
--rw-r--r--   0 runner    (1001) docker     (116)     1506 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdsInsightsEdgeStoreVisitsAdCampaignInsights.py
--rw-r--r--   0 runner    (1001) docker     (116)     1647 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdsPixelEventsPost.py
--rw-r--r--   0 runner    (1001) docker     (116)     2007 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdsPixelEventsPostCustom.py
--rw-r--r--   0 runner    (1001) docker     (116)     1489 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdsPixelSharedAccountsEdge.py
--rw-r--r--   0 runner    (1001) docker     (116)     1464 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdsPixelSharedAccountsPost.py
--rw-r--r--   0 runner    (1001) docker     (116)     1457 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/AdsPixelSharedAgenciesEdge.py
--rw-r--r--   0 runner    (1001) docker     (116)     1549 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/BusinessOwnedProductCatalogsPostDestinationCatalog.py
--rw-r--r--   0 runner    (1001) docker     (116)     1539 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/BusinessOwnedProductCatalogsPostFlightCatalog.py
--rw-r--r--   0 runner    (1001) docker     (116)     1537 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/BusinessOwnedProductCatalogsPostHotelCatalog.py
--rw-r--r--   0 runner    (1001) docker     (116)     1507 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/BusinessOwnedProductCatalogsPostProductCatalog.py
--rw-r--r--   0 runner    (1001) docker     (116)     1484 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/CustomAudienceDelete.py
--rw-r--r--   0 runner    (1001) docker     (116)     1411 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/CustomAudienceNode.py
--rw-r--r--   0 runner    (1001) docker     (116)     1431 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/CustomAudienceNodeReadRule.py
--rw-r--r--   0 runner    (1001) docker     (116)     1447 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/CustomAudiencePost.py
--rw-r--r--   0 runner    (1001) docker     (116)     1772 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/CustomAudienceUsersPost.py
--rw-r--r--   0 runner    (1001) docker     (116)     1853 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/CustomAudienceUsersPostCrossPlatform.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/MultiPageFeedCreateThenDelete.py
--rw-r--r--   0 runner    (1001) docker     (116)     4218 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/MultiPromoteYourPage.py
--rw-r--r--   0 runner    (1001) docker     (116)     1602 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/OfflineConversionsCreateOfflineSet.py
--rw-r--r--   0 runner    (1001) docker     (116)     1433 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/PageFeedEdge.py
--rw-r--r--   0 runner    (1001) docker     (116)     1473 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/PageFeedPost.py
--rw-r--r--   0 runner    (1001) docker     (116)     1571 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/PageFeedPostFeedImageDeepLink.py
--rw-r--r--   0 runner    (1001) docker     (116)     1466 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/PageNode.py
--rw-r--r--   0 runner    (1001) docker     (116)     1454 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/PageNodePageSearch.py
--rw-r--r--   0 runner    (1001) docker     (116)     1429 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/PagePhotosEdge.py
--rw-r--r--   0 runner    (1001) docker     (116)     1519 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/PagePhotosPost.py
--rw-r--r--   0 runner    (1001) docker     (116)     1479 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/PagePictureEdge.py
--rw-r--r--   0 runner    (1001) docker     (116)     1452 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/PagePostCommentsEdge.py
--rw-r--r--   0 runner    (1001) docker     (116)     1491 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/PagePostCommentsPost.py
--rw-r--r--   0 runner    (1001) docker     (116)     1460 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/PagePostDelete.py
--rw-r--r--   0 runner    (1001) docker     (116)     1387 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/PagePostNode.py
--rw-r--r--   0 runner    (1001) docker     (116)     1427 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/PagePostPost.py
--rw-r--r--   0 runner    (1001) docker     (116)     1434 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/PagePostsEdge.py
--rw-r--r--   0 runner    (1001) docker     (116)     1944 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/PagePostsEdgePagePostCreateCarousel.py
--rw-r--r--   0 runner    (1001) docker     (116)     1426 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/PageRolesEdge.py
--rw-r--r--   0 runner    (1001) docker     (116)     1422 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/PageSubscribedAppsPost.py
--rw-r--r--   0 runner    (1001) docker     (116)     1497 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/ProductCatalogEventStatsEdge.py
--rw-r--r--   0 runner    (1001) docker     (116)     2178 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/ProductCatalogHotelsPost.py
--rw-r--r--   0 runner    (1001) docker     (116)     1479 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/ProductCatalogHotelsPostUpdateHotelsCatalogSettings.py
--rw-r--r--   0 runner    (1001) docker     (116)     1609 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/ProductCatalogProductFeedsPostProductFeed.py
--rw-r--r--   0 runner    (1001) docker     (116)     1569 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/ProductCatalogProductSetsPostHotelSet.py
--rw-r--r--   0 runner    (1001) docker     (116)     1563 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/ProductCatalogProductSetsPostProductSet.py
--rw-r--r--   0 runner    (1001) docker     (116)     2356 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/ServerSideApi.py
--rw-r--r--   0 runner    (1001) docker     (116)     1440 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/UserAccountsEdge.py
--rw-r--r--   0 runner    (1001) docker     (116)     1453 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/UserAdAccountsEdge.py
--rw-r--r--   0 runner    (1001) docker     (116)     1370 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/UserLeadGenInfoNode.py
--rw-r--r--   0 runner    (1001) docker     (116)     1370 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/UserNode.py
--rw-r--r--   0 runner    (1001) docker     (116)     1461 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/VideoThumbnailsEdge.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5482 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/ad_creation_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     2039 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/async.py
--rw-r--r--   0 runner    (1001) docker     (116)     3388 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/batch_create.py
--rw-r--r--   0 runner    (1001) docker     (116)     3887 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/batch_pause.py
--rw-r--r--   0 runner    (1001) docker     (116)     1422 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/batch_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     5708 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/custom_audience_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-14 01:49:23.192526 facebook_business-9.0.2/examples/dpa-update/
--rw-r--r--   0 runner    (1001) docker     (116)     2199 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/dpa-update/dpa_search.py
--rw-r--r--   0 runner    (1001) docker     (116)     2745 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/dpa-update/dpa_update.py
--rw-r--r--   0 runner    (1001) docker     (116)     3031 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/dpa-update/stock_update.py
--rw-r--r--   0 runner    (1001) docker     (116)     1122 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/my_app_session.cfg.dist
--rw-r--r--   0 runner    (1001) docker     (116)     3022 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/read_objects.py
--rw-r--r--   0 runner    (1001) docker     (116)     3315 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/simple_create.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     5793 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/test.png
--rw-r--r--   0 runner    (1001) docker     (116)     2111 2021-01-14 01:49:10.000000 facebook_business-9.0.2/examples/upload_video.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-14 01:49:23.192526 facebook_business-9.0.2/facebook_business/
--rw-r--r--   0 runner    (1001) docker     (116)     1225 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-14 01:49:23.248526 facebook_business-9.0.2/facebook_business/adobjects/
--rw-r--r--   0 runner    (1001) docker     (116)     1043 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    22555 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/abstractcrudobject.py
--rw-r--r--   0 runner    (1001) docker     (116)     5510 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/abstractobject.py
--rw-r--r--   0 runner    (1001) docker     (116)    29480 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/ad.py
--rw-r--r--   0 runner    (1001) docker     (116)   156084 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adaccount.py
--rw-r--r--   0 runner    (1001) docker     (116)     5173 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adaccountactivity.py
--rw-r--r--   0 runner    (1001) docker     (116)     3146 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adaccountadruleshistory.py
--rw-r--r--   0 runner    (1001) docker     (116)     4039 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adaccountadvolume.py
--rw-r--r--   0 runner    (1001) docker     (116)     2115 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adaccountcontentfilterlevelsinheritance.py
--rw-r--r--   0 runner    (1001) docker     (116)     1908 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adaccountdefaultdestination.py
--rw-r--r--   0 runner    (1001) docker     (116)     3830 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adaccountdefaultobjective.py
--rw-r--r--   0 runner    (1001) docker     (116)     3299 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adaccountdeliveryestimate.py
--rw-r--r--   0 runner    (1001) docker     (116)     2991 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adaccountmatchedsearchapplicationsedgedata.py
--rw-r--r--   0 runner    (1001) docker     (116)     1767 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adaccountmaxbid.py
--rw-r--r--   0 runner    (1001) docker     (116)     2028 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adaccountpromotableobjects.py
--rw-r--r--   0 runner    (1001) docker     (116)     1858 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adaccountreachestimate.py
--rw-r--r--   0 runner    (1001) docker     (116)     1947 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adaccountrecommendedcamapaignbudget.py
--rw-r--r--   0 runner    (1001) docker     (116)     3544 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adaccountroas.py
--rw-r--r--   0 runner    (1001) docker     (116)     2622 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adaccountsubscribedapps.py
--rw-r--r--   0 runner    (1001) docker     (116)    12448 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adaccounttargetingunified.py
--rw-r--r--   0 runner    (1001) docker     (116)     1824 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adaccounttrackingdata.py
--rw-r--r--   0 runner    (1001) docker     (116)     2361 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adaccountuser.py
--rw-r--r--   0 runner    (1001) docker     (116)     7902 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adactivity.py
--rw-r--r--   0 runner    (1001) docker     (116)     5538 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adassetfeedspec.py
--rw-r--r--   0 runner    (1001) docker     (116)     2108 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adassetfeedspecassetlabel.py
--rw-r--r--   0 runner    (1001) docker     (116)     1918 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adassetfeedspecbody.py
--rw-r--r--   0 runner    (1001) docker     (116)     1927 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adassetfeedspeccaption.py
--rw-r--r--   0 runner    (1001) docker     (116)     1939 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adassetfeedspecdescription.py
--rw-r--r--   0 runner    (1001) docker     (116)     2386 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adassetfeedspecgrouprule.py
--rw-r--r--   0 runner    (1001) docker     (116)     2042 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adassetfeedspecimage.py
--rw-r--r--   0 runner    (1001) docker     (116)     2188 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adassetfeedspeclinkurl.py
--rw-r--r--   0 runner    (1001) docker     (116)     1921 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adassetfeedspectitle.py
--rw-r--r--   0 runner    (1001) docker     (116)     2161 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adassetfeedspecvideo.py
--rw-r--r--   0 runner    (1001) docker     (116)     5368 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adasyncrequest.py
--rw-r--r--   0 runner    (1001) docker     (116)     8927 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adasyncrequestset.py
--rw-r--r--   0 runner    (1001) docker     (116)     1887 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adasyncrequestsetnotificationresult.py
--rw-r--r--   0 runner    (1001) docker     (116)     1926 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adbidadjustments.py
--rw-r--r--   0 runner    (1001) docker     (116)    11910 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcampaignactivity.py
--rw-r--r--   0 runner    (1001) docker     (116)     1824 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcampaignbidconstraint.py
--rw-r--r--   0 runner    (1001) docker     (116)     3303 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcampaigndeliveryestimate.py
--rw-r--r--   0 runner    (1001) docker     (116)     1942 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcampaigndeliverystatsunsupportedreasons.py
--rw-r--r--   0 runner    (1001) docker     (116)     1974 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcampaignfrequencycontrolspecs.py
--rw-r--r--   0 runner    (1001) docker     (116)     6668 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcampaigngroupactivity.py
--rw-r--r--   0 runner    (1001) docker     (116)     2058 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcampaignissuesinfo.py
--rw-r--r--   0 runner    (1001) docker     (116)     2058 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcampaignlearningstageinfo.py
--rw-r--r--   0 runner    (1001) docker     (116)     1995 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcampaignoptimizationevent.py
--rw-r--r--   0 runner    (1001) docker     (116)     1812 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcampaignpacedbidinfo.py
--rw-r--r--   0 runner    (1001) docker     (116)    20514 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcreative.py
--rw-r--r--   0 runner    (1001) docker     (116)     1878 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcreativeaddisclaimer.py
--rw-r--r--   0 runner    (1001) docker     (116)     2005 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcreativecollectionthumbnailinfo.py
--rw-r--r--   0 runner    (1001) docker     (116)     1801 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcreativeinsights.py
--rw-r--r--   0 runner    (1001) docker     (116)     1938 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcreativeinteractivecomponentsspec.py
--rw-r--r--   0 runner    (1001) docker     (116)     5263 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcreativelinkdata.py
--rw-r--r--   0 runner    (1001) docker     (116)     2003 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcreativelinkdataapplinkspec.py
--rw-r--r--   0 runner    (1001) docker     (116)     4283 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcreativelinkdatacalltoaction.py
--rw-r--r--   0 runner    (1001) docker     (116)     2517 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcreativelinkdatacalltoactionvalue.py
--rw-r--r--   0 runner    (1001) docker     (116)     2496 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcreativelinkdatachildattachment.py
--rw-r--r--   0 runner    (1001) docker     (116)     4640 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcreativelinkdataimagelayerspec.py
--rw-r--r--   0 runner    (1001) docker     (116)     5404 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcreativelinkdataimageoverlayspec.py
--rw-r--r--   0 runner    (1001) docker     (116)     1938 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcreativelinkdatasponsorshipinfospec.py
--rw-r--r--   0 runner    (1001) docker     (116)     2035 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcreativelinkdatatemplatevideospec.py
--rw-r--r--   0 runner    (1001) docker     (116)     2285 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcreativeobjectstoryspec.py
--rw-r--r--   0 runner    (1001) docker     (116)     1845 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcreativeomnichannellinkspec.py
--rw-r--r--   0 runner    (1001) docker     (116)     2274 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcreativephotodata.py
--rw-r--r--   0 runner    (1001) docker     (116)     1978 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcreativephotodatamediaelements.py
--rw-r--r--   0 runner    (1001) docker     (116)     2113 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcreativeplacedata.py
--rw-r--r--   0 runner    (1001) docker     (116)     1824 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcreativeplatformcustomization.py
--rw-r--r--   0 runner    (1001) docker     (116)     1848 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcreativeportraitcustomizations.py
--rw-r--r--   0 runner    (1001) docker     (116)     1989 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcreativepostclickconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (116)     1944 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcreativerecommendersettings.py
--rw-r--r--   0 runner    (1001) docker     (116)     2142 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcreativestaticfallbackspec.py
--rw-r--r--   0 runner    (1001) docker     (116)     2121 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcreativetemplateurlspec.py
--rw-r--r--   0 runner    (1001) docker     (116)     1779 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcreativetextdata.py
--rw-r--r--   0 runner    (1001) docker     (116)     3304 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcreativevideodata.py
--rw-r--r--   0 runner    (1001) docker     (116)     2392 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adcustomizationrulespec.py
--rw-r--r--   0 runner    (1001) docker     (116)     1788 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/addynamiccreative.py
--rw-r--r--   0 runner    (1001) docker     (116)     2041 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adentitytargetspend.py
--rw-r--r--   0 runner    (1001) docker     (116)     9428 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adgroupactivity.py
--rw-r--r--   0 runner    (1001) docker     (116)     2049 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adgroupissuesinfo.py
--rw-r--r--   0 runner    (1001) docker     (116)     4583 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adgroupplacementspecificreviewfeedback.py
--rw-r--r--   0 runner    (1001) docker     (116)     2010 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adgrouprelevancescore.py
--rw-r--r--   0 runner    (1001) docker     (116)     1926 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adgroupreviewfeedback.py
--rw-r--r--   0 runner    (1001) docker     (116)     4989 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adimage.py
--rw-r--r--   0 runner    (1001) docker     (116)     2013 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adkeywords.py
--rw-r--r--   0 runner    (1001) docker     (116)    10566 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adlabel.py
--rw-r--r--   0 runner    (1001) docker     (116)     8797 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/admonetizationproperty.py
--rw-r--r--   0 runner    (1001) docker     (116)     2046 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adnetworkanalyticsasyncqueryresult.py
--rw-r--r--   0 runner    (1001) docker     (116)     4776 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adnetworkanalyticssyncqueryresult.py
--rw-r--r--   0 runner    (1001) docker     (116)     4974 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adoptablepet.py
--rw-r--r--   0 runner    (1001) docker     (116)     3581 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adplacement.py
--rw-r--r--   0 runner    (1001) docker     (116)     4633 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adplacepageset.py
--rw-r--r--   0 runner    (1001) docker     (116)     1986 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adplacepagesetmetadata.py
--rw-r--r--   0 runner    (1001) docker     (116)     4064 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adpreview.py
--rw-r--r--   0 runner    (1001) docker     (116)     4465 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adpromotedobject.py
--rw-r--r--   0 runner    (1001) docker     (116)     2539 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adrecommendation.py
--rw-r--r--   0 runner    (1001) docker     (116)     1776 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adrecommendationdata.py
--rw-r--r--   0 runner    (1001) docker     (116)     7655 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adreportrun.py
--rw-r--r--   0 runner    (1001) docker     (116)     4257 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adreportspec.py
--rw-r--r--   0 runner    (1001) docker     (116)    10322 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adrule.py
--rw-r--r--   0 runner    (1001) docker     (116)     2134 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adruleevaluationspec.py
--rw-r--r--   0 runner    (1001) docker     (116)     2055 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adruleexecutionoptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     2590 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adruleexecutionspec.py
--rw-r--r--   0 runner    (1001) docker     (116)     2341 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adrulefilters.py
--rw-r--r--   0 runner    (1001) docker     (116)     2866 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adrulehistory.py
--rw-r--r--   0 runner    (1001) docker     (116)     2127 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adrulehistoryresult.py
--rw-r--r--   0 runner    (1001) docker     (116)     1974 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adrulehistoryresultaction.py
--rw-r--r--   0 runner    (1001) docker     (116)     1893 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adruleschedule.py
--rw-r--r--   0 runner    (1001) docker     (116)     1871 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adruleschedulespec.py
--rw-r--r--   0 runner    (1001) docker     (116)     2711 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adruletrigger.py
--rw-r--r--   0 runner    (1001) docker     (116)     4092 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adsactionstats.py
--rw-r--r--   0 runner    (1001) docker     (116)    43982 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adset.py
--rw-r--r--   0 runner    (1001) docker     (116)     2170 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adsimagecrops.py
--rw-r--r--   0 runner    (1001) docker     (116)    19535 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adsinsights.py
--rw-r--r--   0 runner    (1001) docker     (116)     2011 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adsoptimaldeliverygrowthopportunity.py
--rw-r--r--   0 runner    (1001) docker     (116)    18977 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adspixel.py
--rw-r--r--   0 runner    (1001) docker     (116)     1994 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adspixelstats.py
--rw-r--r--   0 runner    (1001) docker     (116)     2768 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adspixelstatsresult.py
--rw-r--r--   0 runner    (1001) docker     (116)    11827 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adstudy.py
--rw-r--r--   0 runner    (1001) docker     (116)    10324 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adstudycell.py
--rw-r--r--   0 runner    (1001) docker     (116)    13750 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adstudyobjective.py
--rw-r--r--   0 runner    (1001) docker     (116)     2162 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/adstudyobjectiveid.py
--rw-r--r--   0 runner    (1001) docker     (116)    46245 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/advideo.py
--rw-r--r--   0 runner    (1001) docker     (116)     2880 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/agencyclientdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (116)     1794 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/agerange.py
--rw-r--r--   0 runner    (1001) docker     (116)    16166 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/album.py
--rw-r--r--   0 runner    (1001) docker     (116)     1929 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/androidapplink.py
--rw-r--r--   0 runner    (1001) docker     (116)    86267 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/application.py
--rw-r--r--   0 runner    (1001) docker     (116)     4658 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/apprequest.py
--rw-r--r--   0 runner    (1001) docker     (116)     2132 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/apprequestformerrecipient.py
--rw-r--r--   0 runner    (1001) docker     (116)     2194 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/assigneduser.py
--rw-r--r--   0 runner    (1001) docker     (116)     2586 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/asyncrequest.py
--rw-r--r--   0 runner    (1001) docker     (116)     3920 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/asyncsession.py
--rw-r--r--   0 runner    (1001) docker     (116)    18555 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/atlascampaign.py
--rw-r--r--   0 runner    (1001) docker     (116)     1845 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/attributionspec.py
--rw-r--r--   0 runner    (1001) docker     (116)     2319 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/audienceinsightsstudyspec.py
--rw-r--r--   0 runner    (1001) docker     (116)     2180 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/audiencepermissionforactions.py
--rw-r--r--   0 runner    (1001) docker     (116)     4096 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/audiocopyright.py
--rw-r--r--   0 runner    (1001) docker     (116)     4910 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/automotivemodel.py
--rw-r--r--   0 runner    (1001) docker     (116)     1989 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/billedamountdetails.py
--rw-r--r--   0 runner    (1001) docker     (116)     2055 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/brandsafetyblocklistusage.py
--rw-r--r--   0 runner    (1001) docker     (116)     2879 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/broadtargetingcategories.py
--rw-r--r--   0 runner    (1001) docker     (116)   113889 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/business.py
--rw-r--r--   0 runner    (1001) docker     (116)     2126 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/businessadaccountrequest.py
--rw-r--r--   0 runner    (1001) docker     (116)     4700 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/businessagreement.py
--rw-r--r--   0 runner    (1001) docker     (116)     2137 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/businessapplicationrequest.py
--rw-r--r--   0 runner    (1001) docker     (116)    38693 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/businessassetgroup.py
--rw-r--r--   0 runner    (1001) docker     (116)     4930 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/businessassetsharingagreement.py
--rw-r--r--   0 runner    (1001) docker     (116)     3785 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/businessownedobjectonbehalfofrequest.py
--rw-r--r--   0 runner    (1001) docker     (116)     2088 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/businesspagerequest.py
--rw-r--r--   0 runner    (1001) docker     (116)     6955 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/businessrolerequest.py
--rw-r--r--   0 runner    (1001) docker     (116)    20950 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/businessunit.py
--rw-r--r--   0 runner    (1001) docker     (116)    11916 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/businessuser.py
--rw-r--r--   0 runner    (1001) docker     (116)    37089 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/campaign.py
--rw-r--r--   0 runner    (1001) docker     (116)     1965 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/campaigngroupbrandconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (116)     1801 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/campaigngroupcollaborativeadspartnerinfo.py
--rw-r--r--   0 runner    (1001) docker     (116)     8283 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/canvas.py
--rw-r--r--   0 runner    (1001) docker     (116)     2348 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/canvasadsettings.py
--rw-r--r--   0 runner    (1001) docker     (116)     1776 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/canvasbodyelement.py
--rw-r--r--   0 runner    (1001) docker     (116)     1949 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/canvascollectionthumbnail.py
--rw-r--r--   0 runner    (1001) docker     (116)     1821 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/catalogbasedtargeting.py
--rw-r--r--   0 runner    (1001) docker     (116)     1968 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/catalogitemappealstatus.py
--rw-r--r--   0 runner    (1001) docker     (116)     2288 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/catalogitemapplinks.py
--rw-r--r--   0 runner    (1001) docker     (116)     1941 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/catalogitemchannelstointegritystatus.py
--rw-r--r--   0 runner    (1001) docker     (116)     6249 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/catalogsubverticallist.py
--rw-r--r--   0 runner    (1001) docker     (116)     2262 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/checkbatchrequeststatus.py
--rw-r--r--   0 runner    (1001) docker     (116)     2207 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/childevent.py
--rw-r--r--   0 runner    (1001) docker     (116)     1746 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/clicktrackingtag.py
--rw-r--r--   0 runner    (1001) docker     (116)     1786 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/collaborativeadspartnerinfolistitem.py
--rw-r--r--   0 runner    (1001) docker     (116)     4741 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/collaborativeadssharesettings.py
--rw-r--r--   0 runner    (1001) docker     (116)    15975 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/comment.py
--rw-r--r--   0 runner    (1001) docker     (116)    16406 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/commercemerchantsettings.py
--rw-r--r--   0 runner    (1001) docker     (116)     2316 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/commercemerchantsettingssetupstatus.py
--rw-r--r--   0 runner    (1001) docker     (116)    21046 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/commerceorder.py
--rw-r--r--   0 runner    (1001) docker     (116)     4937 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/commerceordertransactiondetail.py
--rw-r--r--   0 runner    (1001) docker     (116)     2049 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/commercepayout.py
--rw-r--r--   0 runner    (1001) docker     (116)     1854 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/commercesettings.py
--rw-r--r--   0 runner    (1001) docker     (116)     2093 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/connectionstargeting.py
--rw-r--r--   0 runner    (1001) docker     (116)     3490 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/contentdeliveryreport.py
--rw-r--r--   0 runner    (1001) docker     (116)     3630 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/conversionactionquery.py
--rw-r--r--   0 runner    (1001) docker     (116)     2894 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/copyrightreferencecontainer.py
--rw-r--r--   0 runner    (1001) docker     (116)     2247 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/coverphoto.py
--rw-r--r--   0 runner    (1001) docker     (116)     3834 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/cpasadvertiserpartnershiprecommendation.py
--rw-r--r--   0 runner    (1001) docker     (116)     4650 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/cpascollaborationrequest.py
--rw-r--r--   0 runner    (1001) docker     (116)     4958 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/cpasparentcatalogsettings.py
--rw-r--r--   0 runner    (1001) docker     (116)     1881 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/creativehistory.py
--rw-r--r--   0 runner    (1001) docker     (116)     1980 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/creditpartitionactionoptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     2020 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/currency.py
--rw-r--r--   0 runner    (1001) docker     (116)     2004 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/currencyamount.py
--rw-r--r--   0 runner    (1001) docker     (116)    25861 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/customaudience.py
--rw-r--r--   0 runner    (1001) docker     (116)     2054 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/customaudienceadaccount.py
--rw-r--r--   0 runner    (1001) docker     (116)     4997 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/customaudiencedatasource.py
--rw-r--r--   0 runner    (1001) docker     (116)     2268 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/customaudiencesession.py
--rw-r--r--   0 runner    (1001) docker     (116)     2121 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/customaudiencesharedaccountinfo.py
--rw-r--r--   0 runner    (1001) docker     (116)     1914 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/customaudiencesharingstatus.py
--rw-r--r--   0 runner    (1001) docker     (116)     1851 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/customaudiencestatus.py
--rw-r--r--   0 runner    (1001) docker     (116)     2144 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/customaudiencestos.py
--rw-r--r--   0 runner    (1001) docker     (116)     9857 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/customconversion.py
--rw-r--r--   0 runner    (1001) docker     (116)     2333 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/customconversionstatsresult.py
--rw-r--r--   0 runner    (1001) docker     (116)     1962 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/customusersettings.py
--rw-r--r--   0 runner    (1001) docker     (116)     2258 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/dacheck.py
--rw-r--r--   0 runner    (1001) docker     (116)     1947 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/daypart.py
--rw-r--r--   0 runner    (1001) docker     (116)     1981 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/deliverycheck.py
--rw-r--r--   0 runner    (1001) docker     (116)     1956 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/deliverycheckextrainfo.py
--rw-r--r--   0 runner    (1001) docker     (116)     3964 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/destination.py
--rw-r--r--   0 runner    (1001) docker     (116)     3249 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/destinationcatalogsettings.py
--rw-r--r--   0 runner    (1001) docker     (116)     3153 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/domain.py
--rw-r--r--   0 runner    (1001) docker     (116)     3221 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/dynamiccontentset.py
--rw-r--r--   0 runner    (1001) docker     (116)     2103 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/dynamicpostchildattachment.py
--rw-r--r--   0 runner    (1001) docker     (116)     3339 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/dynamicpriceconfigbydate.py
--rw-r--r--   0 runner    (1001) docker     (116)     2352 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/engagement.py
--rw-r--r--   0 runner    (1001) docker     (116)     2525 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/entityattextrange.py
--rw-r--r--   0 runner    (1001) docker     (116)    19020 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/event.py
--rw-r--r--   0 runner    (1001) docker     (116)     7290 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/eventsourcegroup.py
--rw-r--r--   0 runner    (1001) docker     (116)     2242 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/experience.py
--rw-r--r--   0 runner    (1001) docker     (116)    11471 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/extendedcredit.py
--rw-r--r--   0 runner    (1001) docker     (116)     6690 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/extendedcreditallocationconfig.py
--rw-r--r--   0 runner    (1001) docker     (116)     9218 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/extendedcreditinvoicegroup.py
--rw-r--r--   0 runner    (1001) docker     (116)     2298 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/externaleventsource.py
--rw-r--r--   0 runner    (1001) docker     (116)     1963 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/fameexportconfig.py
--rw-r--r--   0 runner    (1001) docker     (116)     4002 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/flexibletargeting.py
--rw-r--r--   0 runner    (1001) docker     (116)     5572 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/flight.py
--rw-r--r--   0 runner    (1001) docker     (116)     2242 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/fundingsourcedetails.py
--rw-r--r--   0 runner    (1001) docker     (116)     2003 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/fundingsourcedetailscoupon.py
--rw-r--r--   0 runner    (1001) docker     (116)    48835 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/group.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-14 01:49:23.248526 facebook_business-9.0.2/facebook_business/adobjects/helpers/
--rw-r--r--   0 runner    (1001) docker     (116)     1043 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3343 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/helpers/adaccountmixin.py
--rw-r--r--   0 runner    (1001) docker     (116)     2453 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/helpers/adaccountusermixin.py
--rw-r--r--   0 runner    (1001) docker     (116)     5769 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/helpers/adimagemixin.py
--rw-r--r--   0 runner    (1001) docker     (116)     1167 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/helpers/adpreviewmixin.py
--rw-r--r--   0 runner    (1001) docker     (116)     1518 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/helpers/adreportrunmixin.py
--rw-r--r--   0 runner    (1001) docker     (116)     1656 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/helpers/adsinsightsmixin.py
--rw-r--r--   0 runner    (1001) docker     (116)     1373 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/helpers/businessmixin.py
--rw-r--r--   0 runner    (1001) docker     (116)     9442 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/helpers/customaudiencemixin.py
--rw-r--r--   0 runner    (1001) docker     (116)     4494 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/helpers/productcatalogmixin.py
--rw-r--r--   0 runner    (1001) docker     (116)     2258 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/helpers/reachfrequencypredictionmixin.py
--rw-r--r--   0 runner    (1001) docker     (116)     9229 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/homelisting.py
--rw-r--r--   0 runner    (1001) docker     (116)     8646 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/hotel.py
--rw-r--r--   0 runner    (1001) docker     (116)     6356 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/hotelroom.py
--rw-r--r--   0 runner    (1001) docker     (116)     2051 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/idname.py
--rw-r--r--   0 runner    (1001) docker     (116)     7844 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/igcomment.py
--rw-r--r--   0 runner    (1001) docker     (116)    10072 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/igmedia.py
--rw-r--r--   0 runner    (1001) docker     (116)    14151 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/iguser.py
--rw-r--r--   0 runner    (1001) docker     (116)     3413 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/insightsresult.py
--rw-r--r--   0 runner    (1001) docker     (116)     3264 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/instagraminsightsresult.py
--rw-r--r--   0 runner    (1001) docker     (116)     1847 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/instagraminsightsvalue.py
--rw-r--r--   0 runner    (1001) docker     (116)     8428 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/instagramuser.py
--rw-r--r--   0 runner    (1001) docker     (116)     6547 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/instantarticle.py
--rw-r--r--   0 runner    (1001) docker     (116)     2656 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/instantarticleinsightsqueryresult.py
--rw-r--r--   0 runner    (1001) docker     (116)     2308 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/invoicecampaign.py
--rw-r--r--   0 runner    (1001) docker     (116)     1875 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/iosapplink.py
--rw-r--r--   0 runner    (1001) docker     (116)     1788 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/keyvalue.py
--rw-r--r--   0 runner    (1001) docker     (116)     5405 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/lead.py
--rw-r--r--   0 runner    (1001) docker     (116)     2088 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/leadgenappointmentbookinginfo.py
--rw-r--r--   0 runner    (1001) docker     (116)     2058 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/leadgenconditionalquestionsgroupchoices.py
--rw-r--r--   0 runner    (1001) docker     (116)     1968 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/leadgenconditionalquestionsgroupquestions.py
--rw-r--r--   0 runner    (1001) docker     (116)     2486 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/leadgendraftquestion.py
--rw-r--r--   0 runner    (1001) docker     (116)    10705 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/leadgenform.py
--rw-r--r--   0 runner    (1001) docker     (116)     2028 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/leadgenpostsubmissioncheckresult.py
--rw-r--r--   0 runner    (1001) docker     (116)     2788 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/leadgenquestion.py
--rw-r--r--   0 runner    (1001) docker     (116)     1827 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/leadgenquestionoption.py
--rw-r--r--   0 runner    (1001) docker     (116)     6151 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/lifeevent.py
--rw-r--r--   0 runner    (1001) docker     (116)     6634 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/link.py
--rw-r--r--   0 runner    (1001) docker     (116)    10433 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/liveencoder.py
--rw-r--r--   0 runner    (1001) docker     (116)    21859 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/livevideo.py
--rw-r--r--   0 runner    (1001) docker     (116)     2735 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/livevideoadbreakconfig.py
--rw-r--r--   0 runner    (1001) docker     (116)     3373 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/livevideoerror.py
--rw-r--r--   0 runner    (1001) docker     (116)     3748 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/livevideoinputstream.py
--rw-r--r--   0 runner    (1001) docker     (116)     2033 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/livevideotargeting.py
--rw-r--r--   0 runner    (1001) docker     (116)     2440 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/location.py
--rw-r--r--   0 runner    (1001) docker     (116)     2664 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/lookalikespec.py
--rw-r--r--   0 runner    (1001) docker     (116)     3495 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/mailingaddress.py
--rw-r--r--   0 runner    (1001) docker     (116)    14523 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/measurementuploadevent.py
--rw-r--r--   0 runner    (1001) docker     (116)     6155 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/mediafingerprint.py
--rw-r--r--   0 runner    (1001) docker     (116)     1845 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/messagingfeaturereview.py
--rw-r--r--   0 runner    (1001) docker     (116)     3639 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/messengerdestinationpagewelcomemessage.py
--rw-r--r--   0 runner    (1001) docker     (116)     2500 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/messengerprofile.py
--rw-r--r--   0 runner    (1001) docker     (116)     2328 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/minimumbudget.py
--rw-r--r--   0 runner    (1001) docker     (116)     4206 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/musicvideocopyright.py
--rw-r--r--   0 runner    (1001) docker     (116)    10358 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/nativeoffer.py
--rw-r--r--   0 runner    (1001) docker     (116)     2047 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/nativeofferdiscount.py
--rw-r--r--   0 runner    (1001) docker     (116)     6868 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/nativeofferview.py
--rw-r--r--   0 runner    (1001) docker     (116)     1705 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/nullnode.py
--rw-r--r--   0 runner    (1001) docker     (116)     4050 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/objectparser.py
--rw-r--r--   0 runner    (1001) docker     (116)    22595 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/offlineconversiondataset.py
--rw-r--r--   0 runner    (1001) docker     (116)     3547 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/offsitepixel.py
--rw-r--r--   0 runner    (1001) docker     (116)     3100 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/opengraphcontext.py
--rw-r--r--   0 runner    (1001) docker     (116)     5643 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/oracletransaction.py
--rw-r--r--   0 runner    (1001) docker     (116)     1956 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/outcomepredictionpoint.py
--rw-r--r--   0 runner    (1001) docker     (116)   183277 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/page.py
--rw-r--r--   0 runner    (1001) docker     (116)     3300 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/pageadminnote.py
--rw-r--r--   0 runner    (1001) docker     (116)    10506 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/pagecalltoaction.py
--rw-r--r--   0 runner    (1001) docker     (116)     2231 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/pagecategory.py
--rw-r--r--   0 runner    (1001) docker     (116)     2447 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/pagechangeproposal.py
--rw-r--r--   0 runner    (1001) docker     (116)     1869 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/pageparking.py
--rw-r--r--   0 runner    (1001) docker     (116)     2037 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/pagepaymentoptions.py
--rw-r--r--   0 runner    (1001) docker     (116)    26956 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/pagepost.py
--rw-r--r--   0 runner    (1001) docker     (116)     2272 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/pagerestaurantservices.py
--rw-r--r--   0 runner    (1001) docker     (116)     2049 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/pagerestaurantspecialties.py
--rw-r--r--   0 runner    (1001) docker     (116)     3483 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/pagesavedfilter.py
--rw-r--r--   0 runner    (1001) docker     (116)     1812 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/pagesettings.py
--rw-r--r--   0 runner    (1001) docker     (116)     1803 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/pagestartinfo.py
--rw-r--r--   0 runner    (1001) docker     (116)     1785 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/pagethreadowner.py
--rw-r--r--   0 runner    (1001) docker     (116)     4550 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/pageupcomingchange.py
--rw-r--r--   0 runner    (1001) docker     (116)     6553 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/pageusermessagethreadlabel.py
--rw-r--r--   0 runner    (1001) docker     (116)     4304 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/partnerstudy.py
--rw-r--r--   0 runner    (1001) docker     (116)     7171 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/paymentenginepayment.py
--rw-r--r--   0 runner    (1001) docker     (116)     1782 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/paymentpricepoints.py
--rw-r--r--   0 runner    (1001) docker     (116)     4823 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/paymentsubscription.py
--rw-r--r--   0 runner    (1001) docker     (116)     1995 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/permission.py
--rw-r--r--   0 runner    (1001) docker     (116)     4280 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/persona.py
--rw-r--r--   0 runner    (1001) docker     (116)    15136 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/photo.py
--rw-r--r--   0 runner    (1001) docker     (116)     3243 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/place.py
--rw-r--r--   0 runner    (1001) docker     (116)     3726 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/placetopic.py
--rw-r--r--   0 runner    (1001) docker     (116)     1896 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/platformimagesource.py
--rw-r--r--   0 runner    (1001) docker     (116)     3987 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/playablecontent.py
--rw-r--r--   0 runner    (1001) docker     (116)    27588 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/post.py
--rw-r--r--   0 runner    (1001) docker     (116)     2025 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/privacy.py
--rw-r--r--   0 runner    (1001) docker     (116)    66599 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/productcatalog.py
--rw-r--r--   0 runner    (1001) docker     (116)     3269 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/productcatalogcategory.py
--rw-r--r--   0 runner    (1001) docker     (116)     2010 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/productcataloghotelroomsbatch.py
--rw-r--r--   0 runner    (1001) docker     (116)     1941 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/productcatalogimagesettings.py
--rw-r--r--   0 runner    (1001) docker     (116)     1869 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/productcatalogimagesettingsoperation.py
--rw-r--r--   0 runner    (1001) docker     (116)     2028 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/productcatalogpricingvariablesbatch.py
--rw-r--r--   0 runner    (1001) docker     (116)     2013 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/productcatalogproductsetsbatch.py
--rw-r--r--   0 runner    (1001) docker     (116)     3834 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/producteventstat.py
--rw-r--r--   0 runner    (1001) docker     (116)    28099 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/productfeed.py
--rw-r--r--   0 runner    (1001) docker     (116)     2070 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/productfeedmissingfeeditemreplacement.py
--rw-r--r--   0 runner    (1001) docker     (116)     5789 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/productfeedrule.py
--rw-r--r--   0 runner    (1001) docker     (116)     1921 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/productfeedrulesuggestion.py
--rw-r--r--   0 runner    (1001) docker     (116)     4204 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/productfeedschedule.py
--rw-r--r--   0 runner    (1001) docker     (116)     6808 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/productfeedupload.py
--rw-r--r--   0 runner    (1001) docker     (116)     1923 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/productfeeduploaddiagnosticsreport.py
--rw-r--r--   0 runner    (1001) docker     (116)     6561 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/productfeeduploaderror.py
--rw-r--r--   0 runner    (1001) docker     (116)     1896 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/productfeeduploaderrorreport.py
--rw-r--r--   0 runner    (1001) docker     (116)     3280 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/productfeeduploaderrorsample.py
--rw-r--r--   0 runner    (1001) docker     (116)    12797 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/productgroup.py
--rw-r--r--   0 runner    (1001) docker     (116)    29319 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/productitem.py
--rw-r--r--   0 runner    (1001) docker     (116)     2019 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/productitemcommerceinsights.py
--rw-r--r--   0 runner    (1001) docker     (116)    16493 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/productset.py
--rw-r--r--   0 runner    (1001) docker     (116)     2049 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/productsetmetadata.py
--rw-r--r--   0 runner    (1001) docker     (116)     1899 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/productvariant.py
--rw-r--r--   0 runner    (1001) docker     (116)     5748 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/profile.py
--rw-r--r--   0 runner    (1001) docker     (116)     2592 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/profilepicturesource.py
--rw-r--r--   0 runner    (1001) docker     (116)     9040 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/publisherblocklist.py
--rw-r--r--   0 runner    (1001) docker     (116)     2084 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/rawcustomaudience.py
--rw-r--r--   0 runner    (1001) docker     (116)     2170 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/reachfrequencyactivity.py
--rw-r--r--   0 runner    (1001) docker     (116)     1839 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/reachfrequencyadformat.py
--rw-r--r--   0 runner    (1001) docker     (116)     2283 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/reachfrequencycurvelowerconfidencerange.py
--rw-r--r--   0 runner    (1001) docker     (116)     2283 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/reachfrequencycurveupperconfidencerange.py
--rw-r--r--   0 runner    (1001) docker     (116)     1914 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/reachfrequencydaypart.py
--rw-r--r--   0 runner    (1001) docker     (116)     2309 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/reachfrequencyestimatescurve.py
--rw-r--r--   0 runner    (1001) docker     (116)     2634 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/reachfrequencyestimatesplacementbreakdown.py
--rw-r--r--   0 runner    (1001) docker     (116)    13465 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/reachfrequencyprediction.py
--rw-r--r--   0 runner    (1001) docker     (116)     2535 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/reachfrequencyspec.py
--rw-r--r--   0 runner    (1001) docker     (116)     3269 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/readonlyanalyticsuserpropertyconfig.py
--rw-r--r--   0 runner    (1001) docker     (116)     2267 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/recommendation.py
--rw-r--r--   0 runner    (1001) docker     (116)     6759 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/referral.py
--rw-r--r--   0 runner    (1001) docker     (116)     1842 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/revsharepolicy.py
--rw-r--r--   0 runner    (1001) docker     (116)     1893 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/richmediaelement.py
--rw-r--r--   0 runner    (1001) docker     (116)     6380 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/rtbdynamicpost.py
--rw-r--r--   0 runner    (1001) docker     (116)     3895 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/savedaudience.py
--rw-r--r--   0 runner    (1001) docker     (116)     3399 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/savedmessageresponse.py
--rw-r--r--   0 runner    (1001) docker     (116)     1729 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/securitysettings.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-14 01:49:23.248526 facebook_business-9.0.2/facebook_business/adobjects/serverside/
--rw-r--r--   0 runner    (1001) docker     (116)     1043 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/serverside/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2055 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/serverside/action_source.py
--rw-r--r--   0 runner    (1001) docker     (116)     2919 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/serverside/batch_processor.py
--rw-r--r--   0 runner    (1001) docker     (116)     7470 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/serverside/content.py
--rw-r--r--   0 runner    (1001) docker     (116)    17409 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/serverside/custom_data.py
--rw-r--r--   0 runner    (1001) docker     (116)     1484 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/serverside/delivery_category.py
--rw-r--r--   0 runner    (1001) docker     (116)    14515 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/serverside/event.py
--rw-r--r--   0 runner    (1001) docker     (116)    11336 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/serverside/event_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     4083 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/serverside/event_request_async.py
--rw-r--r--   0 runner    (1001) docker     (116)     4495 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/serverside/event_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1120 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/serverside/gender.py
--rw-r--r--   0 runner    (1001) docker     (116)     1134 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/serverside/http_method.py
--rw-r--r--   0 runner    (1001) docker     (116)     1217 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/serverside/http_service_interface.py
--rw-r--r--   0 runner    (1001) docker     (116)     7004 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/serverside/normalize.py
--rw-r--r--   0 runner    (1001) docker     (116)     1362 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/serverside/request_options.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-14 01:49:23.252527 facebook_business-9.0.2/facebook_business/adobjects/serverside/tests/
--rw-r--r--   0 runner    (1001) docker     (116)     1043 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/serverside/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5169 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/serverside/tests/batch_processor_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     4058 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/serverside/tests/content_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     5279 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/serverside/tests/custom_data_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     3620 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/serverside/tests/event_request_async_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     5815 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/serverside/tests/event_request_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     3586 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/serverside/tests/event_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     5394 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/serverside/tests/normalize_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     2569 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/serverside/tests/user_data_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     2522 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/serverside/tests/util_test.py
--rw-r--r--   0 runner    (1001) docker     (116)    22381 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/serverside/user_data.py
--rw-r--r--   0 runner    (1001) docker     (116)     1675 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/serverside/util.py
--rw-r--r--   0 runner    (1001) docker     (116)     1968 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/splittestwinner.py
--rw-r--r--   0 runner    (1001) docker     (116)     5339 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/storecatalogsettings.py
--rw-r--r--   0 runner    (1001) docker     (116)     8265 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/systemuser.py
--rw-r--r--   0 runner    (1001) docker     (116)     2637 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/tab.py
--rw-r--r--   0 runner    (1001) docker     (116)    10567 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/targeting.py
--rw-r--r--   0 runner    (1001) docker     (116)     2304 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/targetingdynamicrule.py
--rw-r--r--   0 runner    (1001) docker     (116)     3755 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/targetinggeolocation.py
--rw-r--r--   0 runner    (1001) docker     (116)     2142 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/targetinggeolocationcity.py
--rw-r--r--   0 runner    (1001) docker     (116)     2679 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/targetinggeolocationcustomlocation.py
--rw-r--r--   0 runner    (1001) docker     (116)     2019 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/targetinggeolocationelectoraldistrict.py
--rw-r--r--   0 runner    (1001) docker     (116)     2028 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/targetinggeolocationgeoentities.py
--rw-r--r--   0 runner    (1001) docker     (116)     1815 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/targetinggeolocationlocationcluster.py
--rw-r--r--   0 runner    (1001) docker     (116)     1834 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/targetinggeolocationlocationexpansion.py
--rw-r--r--   0 runner    (1001) docker     (116)     1965 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/targetinggeolocationmarket.py
--rw-r--r--   0 runner    (1001) docker     (116)     2280 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/targetinggeolocationplace.py
--rw-r--r--   0 runner    (1001) docker     (116)     2019 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/targetinggeolocationpoliticaldistrict.py
--rw-r--r--   0 runner    (1001) docker     (116)     1896 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/targetinggeolocationregion.py
--rw-r--r--   0 runner    (1001) docker     (116)     2025 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/targetinggeolocationzip.py
--rw-r--r--   0 runner    (1001) docker     (116)     2024 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/targetingproductaudiencespec.py
--rw-r--r--   0 runner    (1001) docker     (116)     1896 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/targetingproductaudiencesubspec.py
--rw-r--r--   0 runner    (1001) docker     (116)     1815 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/targetingprospectingaudience.py
--rw-r--r--   0 runner    (1001) docker     (116)     1794 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/targetingrelaxation.py
--rw-r--r--   0 runner    (1001) docker     (116)     3882 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/targetingsearch.py
--rw-r--r--   0 runner    (1001) docker     (116)     2344 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/targetingsentenceline.py
--rw-r--r--   0 runner    (1001) docker     (116)     4530 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/thirdpartymeasurementreportdataset.py
--rw-r--r--   0 runner    (1001) docker     (116)     2133 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/trackingandconversionwithdefaults.py
--rw-r--r--   0 runner    (1001) docker     (116)     5266 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/unifiedthread.py
--rw-r--r--   0 runner    (1001) docker     (116)     5025 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/url.py
--rw-r--r--   0 runner    (1001) docker     (116)    85825 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/user.py
--rw-r--r--   0 runner    (1001) docker     (116)     1882 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/usercoverphoto.py
--rw-r--r--   0 runner    (1001) docker     (116)     1800 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/userdevice.py
--rw-r--r--   0 runner    (1001) docker     (116)     2071 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/useridforapp.py
--rw-r--r--   0 runner    (1001) docker     (116)     2070 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/useridforpage.py
--rw-r--r--   0 runner    (1001) docker     (116)     1893 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/userleadgendisclaimerresponse.py
--rw-r--r--   0 runner    (1001) docker     (116)     1836 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/userleadgenfielddata.py
--rw-r--r--   0 runner    (1001) docker     (116)     2070 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/userpaymentmobilepricepoints.py
--rw-r--r--   0 runner    (1001) docker     (116)     2156 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/valuebasedeligiblesource.py
--rw-r--r--   0 runner    (1001) docker     (116)    11759 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/vehicle.py
--rw-r--r--   0 runner    (1001) docker     (116)     5455 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/vehicleoffer.py
--rw-r--r--   0 runner    (1001) docker     (116)     6669 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/videocopyright.py
--rw-r--r--   0 runner    (1001) docker     (116)     1959 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/videocopyrightconditiongroup.py
--rw-r--r--   0 runner    (1001) docker     (116)     1923 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/videocopyrightgeogate.py
--rw-r--r--   0 runner    (1001) docker     (116)     3777 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/videocopyrightrule.py
--rw-r--r--   0 runner    (1001) docker     (116)     1963 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/videocopyrightsegment.py
--rw-r--r--   0 runner    (1001) docker     (116)     4750 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/videolist.py
--rw-r--r--   0 runner    (1001) docker     (116)     6379 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/videopoll.py
--rw-r--r--   0 runner    (1001) docker     (116)     2484 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/videothumbnail.py
--rw-r--r--   0 runner    (1001) docker     (116)     1824 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/videouploadlimits.py
--rw-r--r--   0 runner    (1001) docker     (116)     2231 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/voipinfo.py
--rw-r--r--   0 runner    (1001) docker     (116)     1822 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/webapplink.py
--rw-r--r--   0 runner    (1001) docker     (116)    17207 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/whatsappbusinessaccount.py
--rw-r--r--   0 runner    (1001) docker     (116)     4293 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/whatsappbusinessprofile.py
--rw-r--r--   0 runner    (1001) docker     (116)     1962 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/windowsapplink.py
--rw-r--r--   0 runner    (1001) docker     (116)     1884 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/windowsphoneapplink.py
--rw-r--r--   0 runner    (1001) docker     (116)     1853 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/adobjects/workuserfrontline.py
--rw-r--r--   0 runner    (1001) docker     (116)    30473 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1140 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/apiconfig.py
--rw-r--r--   0 runner    (1001) docker     (116)     3589 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (116)     3527 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/crashreporter.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-14 01:49:23.252527 facebook_business-9.0.2/facebook_business/docs_runner/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/docs_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3069 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/docs_runner/doc_runner.py
--rw-r--r--   0 runner    (1001) docker     (116)     1322 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/docs_runner/get_version.py
--rw-r--r--   0 runner    (1001) docker     (116)     5577 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     1161 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/exit_codes.py
--rw-r--r--   0 runner    (1001) docker     (116)   252975 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/fb_ca_chain_bundle.crt
--rw-r--r--   0 runner    (1001) docker     (116)     6363 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/mixins.py
--rw-r--r--   0 runner    (1001) docker     (116)     3165 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/session.py
--rw-r--r--   0 runner    (1001) docker     (116)     2697 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/specs.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-14 01:49:23.252527 facebook_business-9.0.2/facebook_business/test/
--rw-r--r--   0 runner    (1001) docker     (116)       20 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    24067 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/test/docs.py
--rw-r--r--   0 runner    (1001) docker     (116)    10163 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/test/docs_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)    12391 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/test/integration_ad.py
--rw-r--r--   0 runner    (1001) docker     (116)    16040 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/test/integration_adaccount.py
--rw-r--r--   0 runner    (1001) docker     (116)     9994 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/test/integration_adcreative.py
--rw-r--r--   0 runner    (1001) docker     (116)    10620 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/test/integration_adset.py
--rw-r--r--   0 runner    (1001) docker     (116)    12676 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/test/integration_campaign.py
--rw-r--r--   0 runner    (1001) docker     (116)     9574 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/test/integration_constant.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     2301 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/test/integration_test_runner.py
--rw-r--r--   0 runner    (1001) docker     (116)     2061 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/test/integration_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-14 01:49:23.252527 facebook_business-9.0.2/facebook_business/test/misc/
--rwxr-xr-x   0 runner    (1001) docker     (116)     6620 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/test/misc/image.png
--rw-r--r--   0 runner    (1001) docker     (116)     2487 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/test/other_docs.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     5793 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/test/test.png
--rw-r--r--   0 runner    (1001) docker     (116)    15349 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/test/unit.py
--rw-r--r--   0 runner    (1001) docker     (116)     8461 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/typechecker.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-14 01:49:23.252527 facebook_business-9.0.2/facebook_business/utils/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1323 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/utils/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     1825 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/utils/urls.py
--rw-r--r--   0 runner    (1001) docker     (116)     1603 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/utils/version.py
--rw-r--r--   0 runner    (1001) docker     (116)    12724 2021-01-14 01:49:10.000000 facebook_business-9.0.2/facebook_business/video_uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-14 01:49:23.192526 facebook_business-9.0.2/facebook_business.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    21400 2021-01-14 01:49:22.000000 facebook_business-9.0.2/facebook_business.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    31749 2021-01-14 01:49:23.000000 facebook_business-9.0.2/facebook_business.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-14 01:49:22.000000 facebook_business-9.0.2/facebook_business.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      133 2021-01-14 01:49:22.000000 facebook_business-9.0.2/facebook_business.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       18 2021-01-14 01:49:22.000000 facebook_business-9.0.2/facebook_business.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       45 2021-01-14 01:49:10.000000 facebook_business-9.0.2/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (116)      135 2021-01-14 01:49:10.000000 facebook_business-9.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-01-14 01:49:23.256527 facebook_business-9.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2634 2021-01-14 01:49:10.000000 facebook_business-9.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-16 23:49:27.834138 facebook_business-9.0.3/
+-rw-r--r--   0 runner    (1001) docker     (121)     3352 2021-02-16 23:49:19.000000 facebook_business-9.0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)      249 2021-02-16 23:49:19.000000 facebook_business-9.0.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1895 2021-02-16 23:49:19.000000 facebook_business-9.0.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1045 2021-02-16 23:49:19.000000 facebook_business-9.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1166 2021-02-16 23:49:19.000000 facebook_business-9.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    21400 2021-02-16 23:49:27.834138 facebook_business-9.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    17278 2021-02-16 23:49:19.000000 facebook_business-9.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-16 23:49:27.746138 facebook_business-9.0.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1413 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountActivityNode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1476 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdCreativesEdge.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1544 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdCreativesPost.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1650 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdCreativesPost2CreateAdCreativeLinkAd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1703 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdCreativesPost2CreateLinkAdCallToActionAppInstall.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1671 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdCreativesPost2CreateLinkAdImageCrop.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1898 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdCreativesPost2CreateMAIDPA.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1712 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdCreativesPost2CreateVideoLeadAd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1673 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdCreativesPost2CreateVideoPageLikeAd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1715 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdCreativesPost3CreateAdCreativePageLike.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1976 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdCreativesPost3CreateAssetFeedSpec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2363 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdCreativesPost3CreateCarouselCallToActionAppInstall.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2290 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdCreativesPost3CreateDynamicAdCustomization.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1510 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdCreativesPostCreateAdCreative.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1673 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdCreativesPostCreateAdCreativeCanvas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1972 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdCreativesPostCreateAdCreativeCustomizationCanvasDV.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1981 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdCreativesPostCreateAdCreativeCustomizationCanvasImage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2043 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdCreativesPostCreateAdCreativeCustomizationCanvasVideo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1950 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdSetsPost2CreateMAIA.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1945 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdSetsPostAdSetCreateCpa.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2002 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdSetsPostAdSetCreateCpaAppEvents.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1833 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdSetsPostBehaviorTargeting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1941 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdSetsPostBidMultiplier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2220 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdSetsPostCreateAdSet.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1809 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdSetsPostCreateAudienceNetwork.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1840 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdSetsPostDailyBudget20.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2194 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdSetsPostDemographicTargeting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2092 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdSetsPostInterestTargeting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1898 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdSetsPostLifetimeBudget200Duration10Days.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1941 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdSetsPostOfferClaim.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2164 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdSetsPostOptimizePostEngagement.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1792 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdSetsPostPageLikes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1798 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdSetsPostPlacementTargeting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1846 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdSetsPostReach.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1486 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdVideosPost.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1397 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdsPixelEdgeGetPixelCode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1488 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdsPixelsPost.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1559 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdsPost.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1601 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdsPostAdsRedownload.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1724 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdsPostOfferClaim.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1656 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountAdsPostTrackingPostEngagement.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1527 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountCampaignsEdge.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1578 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountCampaignsPostConversions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1585 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountCampaignsPostEventResponses.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1586 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountCampaignsPostLeadGen.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1569 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountCampaignsPostLinkClicks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1569 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountCampaignsPostLocalAwareness.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1587 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountCampaignsPostMAIA.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1605 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountCampaignsPostMAIDPA.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1583 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountCampaignsPostOfferClaims.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1574 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountCampaignsPostPageLikes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1579 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountCampaignsPostPostEngagement.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1626 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountCampaignsPostStoreCampaign.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1578 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountCampaignsPostVideoViews.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1486 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountCustomAudiencesEdge.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1508 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountCustomAudiencesEdgeDataSourceSubtype.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1642 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountCustomAudiencesPostCreateCustomAudience.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1703 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountCustomAudiencesPostDynamicEventValueBasedLookalikeCustomAudience.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1675 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountCustomAudiencesPostDynamicValueBasedLookalikeCustomAudience.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1775 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountCustomAudiencesPostPlatformCustomAudienceMACARule.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2001 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountCustomAudiencesPostPlatformECAExclusions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1835 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountCustomAudiencesPostPlatformECAMultiFilters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1811 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountCustomAudiencesPostPlatformECAMultiPages.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1778 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountCustomAudiencesPostPlatformEngagementCustomAudience.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1772 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountCustomAudiencesPostPlatformWebsiteCustomAudience.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1620 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountCustomAudiencesPostValueBasedCustomAudience.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1670 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountCustomAudiencesPostValueBasedLookalikeCustomAudience.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1532 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountGeneratePreviewsEdge.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1564 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountGeneratePreviewsEdgeDesktopWithStoryId.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1776 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountGeneratePreviewsEdgeInstagramStandards.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1743 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountGeneratePreviewsEdgeMaiaWithObjectStorySpec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1401 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountNode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1775 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountProductAudiencesPostIphoneViewNoPurchase.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1786 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountProductAudiencesPostNoPurchase.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1578 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdAccountReachEstimate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1395 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdCampaignActivityNode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1404 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdCampaignGroupActivityNode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1449 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdCampaignGroupAdsEdge.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1485 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdCampaignGroupAdsEdgeAdgroupsWithStatusArchived.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1528 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdCampaignGroupAdsetsEdge.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1395 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdCampaignNode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1547 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdCampaignPost.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1558 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdCampaignPostAdsetUpdateCpa.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1517 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdCreativeCreativeInsightsEdge.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1416 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdCreativeNode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1426 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdCreativeNodeRead.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1424 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdCreativeNodeReadInstagramPermalinkUrl.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1547 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdCreativePreviewsEdge.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1504 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdCreativePreviewsEdgePreview.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1547 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdCreativePreviewsEdgePreviewDynamicAds.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1611 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdCreativePreviewsEdgePreviewDynamicAdsWithCustomizations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1425 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdgroupActivityNode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1424 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdgroupLeadsEdgeAdgroupLeads.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1462 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdgroupLeadsEdgeAdgroupLeadsDPA.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1512 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdgroupLeadsEdgeAdgroupLeadsFiltered.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1393 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdgroupPost.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1400 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdgroupPostUpdateStatus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1502 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdsInsightsEdgeAdCampaignInsights.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1506 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdsInsightsEdgeStoreVisitsAdCampaignInsights.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1647 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdsPixelEventsPost.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2384 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdsPixelEventsPostCustom.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1489 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdsPixelSharedAccountsEdge.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1464 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdsPixelSharedAccountsPost.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1457 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/AdsPixelSharedAgenciesEdge.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1549 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/BusinessOwnedProductCatalogsPostDestinationCatalog.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1539 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/BusinessOwnedProductCatalogsPostFlightCatalog.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1537 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/BusinessOwnedProductCatalogsPostHotelCatalog.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1507 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/BusinessOwnedProductCatalogsPostProductCatalog.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1484 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/CustomAudienceDelete.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1411 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/CustomAudienceNode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1431 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/CustomAudienceNodeReadRule.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1447 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/CustomAudiencePost.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1772 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/CustomAudienceUsersPost.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1853 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/CustomAudienceUsersPostCrossPlatform.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2161 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/MultiPageFeedCreateThenDelete.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4218 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/MultiPromoteYourPage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1602 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/OfflineConversionsCreateOfflineSet.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1433 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/PageFeedEdge.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1473 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/PageFeedPost.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1571 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/PageFeedPostFeedImageDeepLink.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1466 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/PageNode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1454 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/PageNodePageSearch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1429 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/PagePhotosEdge.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1519 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/PagePhotosPost.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1479 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/PagePictureEdge.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1452 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/PagePostCommentsEdge.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1491 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/PagePostCommentsPost.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1460 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/PagePostDelete.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1387 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/PagePostNode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1427 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/PagePostPost.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1434 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/PagePostsEdge.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1944 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/PagePostsEdgePagePostCreateCarousel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1426 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/PageRolesEdge.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1422 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/PageSubscribedAppsPost.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1497 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/ProductCatalogEventStatsEdge.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2178 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/ProductCatalogHotelsPost.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1479 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/ProductCatalogHotelsPostUpdateHotelsCatalogSettings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1609 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/ProductCatalogProductFeedsPostProductFeed.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1569 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/ProductCatalogProductSetsPostHotelSet.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1563 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/ProductCatalogProductSetsPostProductSet.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2356 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/ServerSideApi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1440 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/UserAccountsEdge.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1453 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/UserAdAccountsEdge.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1370 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/UserLeadGenInfoNode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1370 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/UserNode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1461 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/VideoThumbnailsEdge.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5482 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/ad_creation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2039 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/async.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3388 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/batch_create.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3887 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/batch_pause.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1422 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/batch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5708 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/custom_audience_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-16 23:49:27.746138 facebook_business-9.0.3/examples/dpa-update/
+-rw-r--r--   0 runner    (1001) docker     (121)     2199 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/dpa-update/dpa_search.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2745 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/dpa-update/dpa_update.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3031 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/dpa-update/stock_update.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1122 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/my_app_session.cfg.dist
+-rw-r--r--   0 runner    (1001) docker     (121)     3022 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/read_objects.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3315 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/simple_create.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5793 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/test.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2111 2021-02-16 23:49:19.000000 facebook_business-9.0.3/examples/upload_video.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-16 23:49:27.750138 facebook_business-9.0.3/facebook_business/
+-rw-r--r--   0 runner    (1001) docker     (121)     1225 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-16 23:49:27.826138 facebook_business-9.0.3/facebook_business/adobjects/
+-rw-r--r--   0 runner    (1001) docker     (121)     1043 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22555 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/abstractcrudobject.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5510 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/abstractobject.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29480 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/ad.py
+-rw-r--r--   0 runner    (1001) docker     (121)   154759 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adaccount.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5173 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adaccountactivity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3146 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adaccountadruleshistory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4039 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adaccountadvolume.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2115 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adaccountcontentfilterlevelsinheritance.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1908 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adaccountdefaultdestination.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3830 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adaccountdefaultobjective.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3299 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adaccountdeliveryestimate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2991 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adaccountmatchedsearchapplicationsedgedata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1767 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adaccountmaxbid.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2028 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adaccountpromotableobjects.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1858 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adaccountreachestimate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1947 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adaccountrecommendedcamapaignbudget.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2622 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adaccountsubscribedapps.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12408 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adaccounttargetingunified.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1824 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adaccounttrackingdata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2361 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adaccountuser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7902 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adactivity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5637 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adassetfeedspec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2108 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adassetfeedspecassetlabel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1918 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adassetfeedspecbody.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1927 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adassetfeedspeccaption.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1939 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adassetfeedspecdescription.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2386 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adassetfeedspecgrouprule.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2042 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adassetfeedspecimage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2188 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adassetfeedspeclinkurl.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1921 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adassetfeedspectitle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2161 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adassetfeedspecvideo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5368 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adasyncrequest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8927 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adasyncrequestset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1887 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adasyncrequestsetnotificationresult.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1926 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adbidadjustments.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12074 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcampaignactivity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1824 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcampaignbidconstraint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3303 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcampaigndeliveryestimate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1942 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcampaigndeliverystatsunsupportedreasons.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1974 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcampaignfrequencycontrolspecs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6668 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcampaigngroupactivity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2058 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcampaignissuesinfo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2058 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcampaignlearningstageinfo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1995 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcampaignoptimizationevent.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1812 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcampaignpacedbidinfo.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20514 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcreative.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1878 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcreativeaddisclaimer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2005 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcreativecollectionthumbnailinfo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1801 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcreativeinsights.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1938 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcreativeinteractivecomponentsspec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5263 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcreativelinkdata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2003 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcreativelinkdataapplinkspec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4283 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcreativelinkdatacalltoaction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2517 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcreativelinkdatacalltoactionvalue.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2496 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcreativelinkdatachildattachment.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4640 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcreativelinkdataimagelayerspec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5404 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcreativelinkdataimageoverlayspec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1938 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcreativelinkdatasponsorshipinfospec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2035 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcreativelinkdatatemplatevideospec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2285 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcreativeobjectstoryspec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1845 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcreativeomnichannellinkspec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2274 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcreativephotodata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1978 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcreativephotodatamediaelements.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2113 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcreativeplacedata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1824 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcreativeplatformcustomization.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1848 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcreativeportraitcustomizations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1989 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcreativepostclickconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1944 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcreativerecommendersettings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2142 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcreativestaticfallbackspec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2121 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcreativetemplateurlspec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1779 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcreativetextdata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3304 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcreativevideodata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2392 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adcustomizationrulespec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1788 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/addynamiccreative.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2041 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adentitytargetspend.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9428 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adgroupactivity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2049 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adgroupissuesinfo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4662 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adgroupplacementspecificreviewfeedback.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2010 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adgrouprelevancescore.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1926 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adgroupreviewfeedback.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4989 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adimage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2013 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adkeywords.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10566 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adlabel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8797 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/admonetizationproperty.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2046 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adnetworkanalyticsasyncqueryresult.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4776 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adnetworkanalyticssyncqueryresult.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4974 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adoptablepet.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3581 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adplacement.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4633 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adplacepageset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1986 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adplacepagesetmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4226 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adpreview.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4465 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adpromotedobject.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2539 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adrecommendation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1776 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adrecommendationdata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7655 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adreportrun.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4257 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adreportspec.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10322 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adrule.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2134 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adruleevaluationspec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2055 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adruleexecutionoptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2590 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adruleexecutionspec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2341 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adrulefilters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2866 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adrulehistory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2127 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adrulehistoryresult.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1974 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adrulehistoryresultaction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1893 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adruleschedule.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1871 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adruleschedulespec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2711 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adruletrigger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4245 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adsactionstats.py
+-rw-r--r--   0 runner    (1001) docker     (121)    44064 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2170 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adsimagecrops.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19628 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adsinsights.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2011 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adsoptimaldeliverygrowthopportunity.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20116 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adspixel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1994 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adspixelstats.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2768 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adspixelstatsresult.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10182 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adstudy.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10324 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adstudycell.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12675 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adstudyobjective.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2162 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/adstudyobjectiveid.py
+-rw-r--r--   0 runner    (1001) docker     (121)    46269 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/advideo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2880 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/agencyclientdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1794 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/agerange.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16166 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/album.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1929 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/androidapplink.py
+-rw-r--r--   0 runner    (1001) docker     (121)    86267 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/application.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4658 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/apprequest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2132 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/apprequestformerrecipient.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2194 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/assigneduser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2586 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/asyncrequest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3920 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/asyncsession.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18555 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/atlascampaign.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1845 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/attributionspec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2319 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/audienceinsightsstudyspec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2180 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/audiencepermissionforactions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4096 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/audiocopyright.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6126 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/automotivemodel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1989 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/billedamountdetails.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2055 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/brandsafetyblocklistusage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2879 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/broadtargetingcategories.py
+-rw-r--r--   0 runner    (1001) docker     (121)   118179 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/business.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2126 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/businessadaccountrequest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4700 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/businessagreement.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2137 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/businessapplicationrequest.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38693 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/businessassetgroup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4930 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/businessassetsharingagreement.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3785 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/businessownedobjectonbehalfofrequest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2088 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/businesspagerequest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6955 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/businessrolerequest.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20950 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/businessunit.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12407 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/businessuser.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37049 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/campaign.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1965 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/campaigngroupbrandconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1801 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/campaigngroupcollaborativeadspartnerinfo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8283 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2348 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/canvasadsettings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1776 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/canvasbodyelement.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1949 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/canvascollectionthumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1821 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/catalogbasedtargeting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1968 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/catalogitemappealstatus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2288 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/catalogitemapplinks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1941 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/catalogitemchannelstointegritystatus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6600 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/catalogsubverticallist.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2262 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/checkbatchrequeststatus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2207 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/childevent.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1746 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/clicktrackingtag.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1786 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/collaborativeadspartnerinfolistitem.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4741 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/collaborativeadssharesettings.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16021 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/comment.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16491 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/commercemerchantsettings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2316 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/commercemerchantsettingssetupstatus.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21046 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/commerceorder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4937 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/commerceordertransactiondetail.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2049 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/commercepayout.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1854 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/commercesettings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2093 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/connectionstargeting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3490 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/contentdeliveryreport.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1788 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/contextualbundlingspec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3630 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/conversionactionquery.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2894 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/copyrightreferencecontainer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2247 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/coverphoto.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3834 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/cpasadvertiserpartnershiprecommendation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4650 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/cpascollaborationrequest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4958 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/cpasparentcatalogsettings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1881 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/creativehistory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1980 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/creditpartitionactionoptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2020 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/currency.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2004 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/currencyamount.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25861 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/customaudience.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2054 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/customaudienceadaccount.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4997 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/customaudiencedatasource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2268 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/customaudiencesession.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2121 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/customaudiencesharedaccountinfo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1914 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/customaudiencesharingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1851 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/customaudiencestatus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2144 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/customaudiencestos.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9857 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/customconversion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2333 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/customconversionstatsresult.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1962 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/customusersettings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2258 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/dacheck.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1947 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/daypart.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1981 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/deliverycheck.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1956 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/deliverycheckextrainfo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3964 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/destination.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3249 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/destinationcatalogsettings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3153 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/domain.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3221 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/dynamiccontentset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2103 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/dynamicpostchildattachment.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3339 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/dynamicpriceconfigbydate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2352 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/engagement.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2525 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/entityattextrange.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19020 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/event.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7290 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/eventsourcegroup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2242 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/experience.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11471 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/extendedcredit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6690 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/extendedcreditallocationconfig.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9218 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/extendedcreditinvoicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2298 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/externaleventsource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1963 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/fameexportconfig.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4002 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/flexibletargeting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5572 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/flight.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2242 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/fundingsourcedetails.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2003 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/fundingsourcedetailscoupon.py
+-rw-r--r--   0 runner    (1001) docker     (121)    48277 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/group.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-16 23:49:27.830138 facebook_business-9.0.3/facebook_business/adobjects/helpers/
+-rw-r--r--   0 runner    (1001) docker     (121)     1043 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3343 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/helpers/adaccountmixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2453 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/helpers/adaccountusermixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5769 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/helpers/adimagemixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1167 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/helpers/adpreviewmixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1518 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/helpers/adreportrunmixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1656 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/helpers/adsinsightsmixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1373 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/helpers/businessmixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9442 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/helpers/customaudiencemixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4494 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/helpers/productcatalogmixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2258 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/helpers/reachfrequencypredictionmixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9229 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/homelisting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8646 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/hotel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6356 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/hotelroom.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2051 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/idname.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7844 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/igcomment.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10072 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/igmedia.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15327 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/iguser.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11311 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/imagecopyright.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3413 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/insightsresult.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3264 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/instagraminsightsresult.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1847 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/instagraminsightsvalue.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8428 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/instagramuser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6547 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/instantarticle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2656 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/instantarticleinsightsqueryresult.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2308 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/invoicecampaign.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1875 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/iosapplink.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1788 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/keyvalue.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5405 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/lead.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2088 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/leadgenappointmentbookinginfo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2058 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/leadgenconditionalquestionsgroupchoices.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1968 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/leadgenconditionalquestionsgroupquestions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2486 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/leadgendraftquestion.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10705 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/leadgenform.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2028 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/leadgenpostsubmissioncheckresult.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2788 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/leadgenquestion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1827 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/leadgenquestionoption.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6151 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/lifeevent.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6634 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/link.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10433 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/liveencoder.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21859 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/livevideo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2735 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/livevideoadbreakconfig.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3373 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/livevideoerror.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3748 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/livevideoinputstream.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2033 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/livevideotargeting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2440 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/location.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2664 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/lookalikespec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3495 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/mailingaddress.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14523 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/measurementuploadevent.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6155 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/mediafingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1845 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/messagingfeaturereview.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3639 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/messengerdestinationpagewelcomemessage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2500 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/messengerprofile.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2328 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/minimumbudget.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4206 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/musicvideocopyright.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10358 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/nativeoffer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2047 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/nativeofferdiscount.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6868 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/nativeofferview.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1705 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/nullnode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4050 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/objectparser.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22595 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/offlineconversiondataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3547 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/offsitepixel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3100 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/opengraphcontext.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5643 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/oracletransaction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1956 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/outcomepredictionpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)   187440 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/page.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3300 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/pageadminnote.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10626 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/pagecalltoaction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2231 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/pagecategory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2447 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/pagechangeproposal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1848 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/pagecommerceeligibility.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1869 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/pageparking.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2037 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/pagepaymentoptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26956 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/pagepost.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2272 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/pagerestaurantservices.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2049 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/pagerestaurantspecialties.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3483 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/pagesavedfilter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1812 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/pagesettings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1803 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/pagestartinfo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1785 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/pagethreadowner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4550 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/pageupcomingchange.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6553 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/pageusermessagethreadlabel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4304 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/partnerstudy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7171 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/paymentenginepayment.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1782 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/paymentpricepoints.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4823 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/paymentsubscription.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1995 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/permission.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4280 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/persona.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15136 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/photo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3243 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/place.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3726 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/placetopic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1896 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/platformimagesource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3987 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/playablecontent.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27588 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/post.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2025 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/privacy.py
+-rw-r--r--   0 runner    (1001) docker     (121)    68280 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/productcatalog.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3269 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/productcatalogcategory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2010 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/productcataloghotelroomsbatch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1941 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/productcatalogimagesettings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1869 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/productcatalogimagesettingsoperation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2028 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/productcatalogpricingvariablesbatch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2013 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/productcatalogproductsetsbatch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3834 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/producteventstat.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28161 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/productfeed.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2070 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/productfeedmissingfeeditemreplacement.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5789 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/productfeedrule.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1921 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/productfeedrulesuggestion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4204 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/productfeedschedule.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6808 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/productfeedupload.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1923 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/productfeeduploaddiagnosticsreport.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6561 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/productfeeduploaderror.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1896 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/productfeeduploaderrorreport.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3280 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/productfeeduploaderrorsample.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11266 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/productgroup.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27903 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/productitem.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2850 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/productitemardata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2019 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/productitemcommerceinsights.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16493 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/productset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2049 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/productsetmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1899 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/productvariant.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5748 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/profile.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2592 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/profilepicturesource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9040 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/publisherblocklist.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2084 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/rawcustomaudience.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2170 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/reachfrequencyactivity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1839 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/reachfrequencyadformat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2283 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/reachfrequencycurvelowerconfidencerange.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2283 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/reachfrequencycurveupperconfidencerange.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1914 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/reachfrequencydaypart.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2309 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/reachfrequencyestimatescurve.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2634 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/reachfrequencyestimatesplacementbreakdown.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13465 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/reachfrequencyprediction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/reachfrequencyspec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2267 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/recommendation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6759 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/referral.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1842 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/revsharepolicy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1893 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/richmediaelement.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6380 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/rtbdynamicpost.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3895 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/savedaudience.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3399 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/savedmessageresponse.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1729 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/securitysettings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-16 23:49:27.830138 facebook_business-9.0.3/facebook_business/adobjects/serverside/
+-rw-r--r--   0 runner    (1001) docker     (121)     1043 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/serverside/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2055 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/serverside/action_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2919 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/serverside/batch_processor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7470 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/serverside/content.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17409 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/serverside/custom_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1484 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/serverside/delivery_category.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14515 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/serverside/event.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11336 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/serverside/event_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4083 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/serverside/event_request_async.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4495 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/serverside/event_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1120 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/serverside/gender.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1134 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/serverside/http_method.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1217 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/serverside/http_service_interface.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7004 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/serverside/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1362 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/serverside/request_options.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-16 23:49:27.834138 facebook_business-9.0.3/facebook_business/adobjects/serverside/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     1043 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/serverside/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5169 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/serverside/tests/batch_processor_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4058 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/serverside/tests/content_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5279 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/serverside/tests/custom_data_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3620 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/serverside/tests/event_request_async_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5815 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/serverside/tests/event_request_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3586 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/serverside/tests/event_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5394 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/serverside/tests/normalize_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2569 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/serverside/tests/user_data_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2522 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/serverside/tests/util_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22381 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/serverside/user_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1675 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/serverside/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1968 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/splittestwinner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5339 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/storecatalogsettings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9618 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/systemuser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2637 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/tab.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10567 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/targeting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2304 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/targetingdynamicrule.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3755 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/targetinggeolocation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2142 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/targetinggeolocationcity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2679 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/targetinggeolocationcustomlocation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2019 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/targetinggeolocationelectoraldistrict.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2028 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/targetinggeolocationgeoentities.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1815 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/targetinggeolocationlocationcluster.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1834 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/targetinggeolocationlocationexpansion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1965 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/targetinggeolocationmarket.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2280 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/targetinggeolocationplace.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2019 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/targetinggeolocationpoliticaldistrict.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1896 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/targetinggeolocationregion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2025 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/targetinggeolocationzip.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2024 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/targetingproductaudiencespec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1896 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/targetingproductaudiencesubspec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1815 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/targetingprospectingaudience.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1794 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/targetingrelaxation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3882 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/targetingsearch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2344 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/targetingsentenceline.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4530 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/thirdpartymeasurementreportdataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2133 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/trackingandconversionwithdefaults.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5266 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/unifiedthread.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5025 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/url.py
+-rw-r--r--   0 runner    (1001) docker     (121)    88225 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/user.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1882 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/usercoverphoto.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1800 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/userdevice.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2071 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/useridforapp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2070 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/useridforpage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1893 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/userleadgendisclaimerresponse.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1836 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/userleadgenfielddata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2070 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/userpaymentmobilepricepoints.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2156 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/valuebasedeligiblesource.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11759 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5455 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/vehicleoffer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6669 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/videocopyright.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1959 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/videocopyrightconditiongroup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1923 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/videocopyrightgeogate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3777 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/videocopyrightrule.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1963 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/videocopyrightsegment.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4750 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/videolist.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6379 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/videopoll.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2484 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/videothumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1824 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/videouploadlimits.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2231 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/voipinfo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1822 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/webapplink.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17207 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/whatsappbusinessaccount.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4293 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/whatsappbusinessprofile.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1962 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/windowsapplink.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1884 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/windowsphoneapplink.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1853 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/adobjects/workuserfrontline.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30473 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1140 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/apiconfig.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3589 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3527 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/crashreporter.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-16 23:49:27.834138 facebook_business-9.0.3/facebook_business/docs_runner/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/docs_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3069 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/docs_runner/doc_runner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1322 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/docs_runner/get_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5577 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1161 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/exit_codes.py
+-rw-r--r--   0 runner    (1001) docker     (121)   252975 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/fb_ca_chain_bundle.crt
+-rw-r--r--   0 runner    (1001) docker     (121)     6363 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3165 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/session.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2697 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/specs.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-16 23:49:27.834138 facebook_business-9.0.3/facebook_business/test/
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24067 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/test/docs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10163 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/test/docs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12391 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/test/integration_ad.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16040 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/test/integration_adaccount.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9994 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/test/integration_adcreative.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10620 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/test/integration_adset.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12676 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/test/integration_campaign.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9574 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/test/integration_constant.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2301 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/test/integration_test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2061 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/test/integration_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-16 23:49:27.834138 facebook_business-9.0.3/facebook_business/test/misc/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6620 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/test/misc/image.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2487 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/test/other_docs.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5793 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/test/test.png
+-rw-r--r--   0 runner    (1001) docker     (121)    15349 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/test/unit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8461 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/typechecker.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-16 23:49:27.834138 facebook_business-9.0.3/facebook_business/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1323 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/utils/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1825 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/utils/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1603 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/utils/version.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12724 2021-02-16 23:49:19.000000 facebook_business-9.0.3/facebook_business/video_uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-16 23:49:27.750138 facebook_business-9.0.3/facebook_business.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    21400 2021-02-16 23:49:27.000000 facebook_business-9.0.3/facebook_business.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    31841 2021-02-16 23:49:27.000000 facebook_business-9.0.3/facebook_business.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-02-16 23:49:27.000000 facebook_business-9.0.3/facebook_business.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      133 2021-02-16 23:49:27.000000 facebook_business-9.0.3/facebook_business.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2021-02-16 23:49:27.000000 facebook_business-9.0.3/facebook_business.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2021-02-16 23:49:19.000000 facebook_business-9.0.3/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      135 2021-02-16 23:49:19.000000 facebook_business-9.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-02-16 23:49:27.834138 facebook_business-9.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2634 2021-02-16 23:49:19.000000 facebook_business-9.0.3/setup.py
```

### Comparing `facebook_business-9.0.2/CHANGELOG.md` & `facebook_business-9.0.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/CONTRIBUTING.md` & `facebook_business-9.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/LICENSE.txt` & `facebook_business-9.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/MANIFEST.in` & `facebook_business-9.0.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/PKG-INFO` & `facebook_business-9.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: facebook_business
-Version: 9.0.2
+Version: 9.0.3
 Summary: Facebook Business SDK
 Home-page: https://github.com/facebook/facebook-python-business-sdk
 Author: Facebook
 Author-email: 
 License: LICENSE.txt
-Download-URL: https://github.com/facebook/facebook-python-business-sdk/tarball/9.0.2
+Download-URL: https://github.com/facebook/facebook-python-business-sdk/tarball/9.0.3
 Description: # Facebook Business SDK for Python
         
         [![Build Status](https://travis-ci.org/facebook/facebook-python-business-sdk.svg)](https://travis-ci.org/facebook/facebook-python-business-sdk)
         
         ### Introduction
         
         The Facebook <a href="https://developers.facebook.com/docs/business-sdk" target="_blank">Business SDK</a> is a one-stop shop to help our partners better serve their businesses. Partners are using multiple Facebook API's to server the needs of their clients. Adopting all these API's and keeping them up to date across the various platforms can be time consuming and ultimately prohibitive. For this reason Facebook has developed the Business SDK bundling many of its APIs into one SDK to ease implementation and upkeep. The Business SDK is an upgraded version of the Marketing API SDK that includes the Marketing API as well as many Facebook APIs from different platforms such as Pages, Business Manager, Instagram, etc.
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: facebook_business Version: 9.0.2 Summary: Facebook
+Metadata-Version: 2.1 Name: facebook_business Version: 9.0.3 Summary: Facebook
 Business SDK Home-page: https://github.com/facebook/facebook-python-business-
 sdk Author: Facebook Author-email: License: LICENSE.txt Download-URL: https://
-github.com/facebook/facebook-python-business-sdk/tarball/9.0.2 Description: #
+github.com/facebook/facebook-python-business-sdk/tarball/9.0.3 Description: #
 Facebook Business SDK for Python [![Build Status](https://travis-ci.org/
 facebook/facebook-python-business-sdk.svg)](https://travis-ci.org/facebook/
 facebook-python-business-sdk) ### Introduction The Facebook Business_SDK is a
 one-stop shop to help our partners better serve their businesses. Partners are
 using multiple Facebook API's to server the needs of their clients. Adopting
 all these API's and keeping them up to date across the various platforms can be
 time consuming and ultimately prohibitive. For this reason Facebook has
```

### Comparing `facebook_business-9.0.2/README.md` & `facebook_business-9.0.3/README.md`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountActivityNode.py` & `facebook_business-9.0.3/examples/AdAccountActivityNode.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountAdCreativesEdge.py` & `facebook_business-9.0.3/examples/AdAccountAdCreativesEdge.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountAdCreativesPost.py` & `facebook_business-9.0.3/examples/AdAccountAdCreativesPost.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountAdCreativesPost2CreateAdCreativeLinkAd.py` & `facebook_business-9.0.3/examples/AdAccountAdCreativesPost2CreateAdCreativeLinkAd.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountAdCreativesPost2CreateLinkAdCallToActionAppInstall.py` & `facebook_business-9.0.3/examples/AdAccountAdCreativesPost2CreateLinkAdCallToActionAppInstall.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountAdCreativesPost2CreateLinkAdImageCrop.py` & `facebook_business-9.0.3/examples/AdAccountAdCreativesPost2CreateLinkAdImageCrop.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountAdCreativesPost2CreateMAIDPA.py` & `facebook_business-9.0.3/examples/AdAccountAdCreativesPost2CreateMAIDPA.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountAdCreativesPost2CreateVideoLeadAd.py` & `facebook_business-9.0.3/examples/AdAccountAdCreativesPost2CreateVideoLeadAd.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountAdCreativesPost2CreateVideoPageLikeAd.py` & `facebook_business-9.0.3/examples/AdAccountAdCreativesPost2CreateVideoPageLikeAd.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountAdCreativesPost3CreateAdCreativePageLike.py` & `facebook_business-9.0.3/examples/AdAccountAdCreativesPost3CreateAdCreativePageLike.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountAdCreativesPost3CreateAssetFeedSpec.py` & `facebook_business-9.0.3/examples/AdAccountAdCreativesPost3CreateAssetFeedSpec.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountAdCreativesPost3CreateCarouselCallToActionAppInstall.py` & `facebook_business-9.0.3/examples/AdAccountAdCreativesPost3CreateCarouselCallToActionAppInstall.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountAdCreativesPost3CreateDynamicAdCustomization.py` & `facebook_business-9.0.3/examples/AdAccountAdCreativesPost3CreateDynamicAdCustomization.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountAdCreativesPostCreateAdCreative.py` & `facebook_business-9.0.3/examples/AdAccountAdCreativesPostCreateAdCreative.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountAdCreativesPostCreateAdCreativeCanvas.py` & `facebook_business-9.0.3/examples/AdAccountAdCreativesPostCreateAdCreativeCanvas.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountAdCreativesPostCreateAdCreativeCustomizationCanvasDV.py` & `facebook_business-9.0.3/examples/AdAccountAdCreativesPostCreateAdCreativeCustomizationCanvasDV.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountAdCreativesPostCreateAdCreativeCustomizationCanvasImage.py` & `facebook_business-9.0.3/examples/AdAccountAdCreativesPostCreateAdCreativeCustomizationCanvasImage.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountAdCreativesPostCreateAdCreativeCustomizationCanvasVideo.py` & `facebook_business-9.0.3/examples/AdAccountAdCreativesPostCreateAdCreativeCustomizationCanvasVideo.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountAdSetsPost2CreateMAIA.py` & `facebook_business-9.0.3/examples/AdAccountAdSetsPost2CreateMAIA.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountAdSetsPostAdSetCreateCpa.py` & `facebook_business-9.0.3/examples/AdAccountAdSetsPostAdSetCreateCpa.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 
 fields = [
 ]
 params = {
   'name': 'A CPA Ad Set',
   'campaign_id': '<adCampaignLinkClicksID>',
   'daily_budget': '5000',
-  'start_time': '2020-12-24T10:13:33-0800',
-  'end_time': '2020-12-31T10:13:33-0800',
+  'start_time': '2021-01-26T14:02:25-0800',
+  'end_time': '2021-02-02T14:02:25-0800',
   'billing_event': 'IMPRESSIONS',
   'optimization_goal': 'REACH',
   'bid_amount': '1000',
   'promoted_object': {'page_id':'<pageID>'},
   'targeting': {'facebook_positions':['feed'],'geo_locations':{'countries':['US']}},
   'user_os': 'iOS',
   'publisher_platforms': 'facebook',
```

### Comparing `facebook_business-9.0.2/examples/AdAccountAdSetsPostAdSetCreateCpaAppEvents.py` & `facebook_business-9.0.3/examples/AdAccountAdSetsPostAdSetCreateCpaAppEvents.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 
 fields = [
 ]
 params = {
   'name': 'A CPA Ad Set optimized for App Events',
   'campaign_id': '<adCampaignAppInstallsID>',
   'daily_budget': '300',
-  'start_time': '2020-12-24T10:14:29-0800',
-  'end_time': '2020-12-31T10:14:29-0800',
+  'start_time': '2021-01-26T14:03:20-0800',
+  'end_time': '2021-02-02T14:03:20-0800',
   'billing_event': 'IMPRESSIONS',
   'optimization_goal': 'OFFSITE_CONVERSIONS',
   'bid_amount': '100',
   'status': 'PAUSED',
   'promoted_object': {'application_id':'<appID>','object_store_url':'<appLink>','custom_event_type':'PURCHASE'},
   'targeting': {'facebook_positions':['feed'],'geo_locations':{'countries':['US']},'user_os':['iOS']},
 }
```

### Comparing `facebook_business-9.0.2/examples/AdAccountAdSetsPostBehaviorTargeting.py` & `facebook_business-9.0.3/examples/AdAccountAdSetsPostBehaviorTargeting.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountAdSetsPostBidMultiplier.py` & `facebook_business-9.0.3/examples/AdAccountAdSetsPostBidMultiplier.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountAdSetsPostCreateAdSet.py` & `facebook_business-9.0.3/examples/AdAccountAdSetsPostCreateAdSet.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 FacebookAdsApi.init(access_token=access_token)
 
 fields = [
 ]
 params = {
   'name': 'My First AdSet',
   'lifetime_budget': '20000',
-  'start_time': '2020-12-24T10:12:46-0800',
-  'end_time': '2020-12-31T10:12:46-0800',
+  'start_time': '2021-01-26T14:01:38-0800',
+  'end_time': '2021-02-02T14:01:38-0800',
   'campaign_id': '<adCampaignLinkClicksID>',
   'bid_amount': '500',
   'billing_event': 'IMPRESSIONS',
   'optimization_goal': 'POST_ENGAGEMENT',
   'targeting': {'age_min':20,'age_max':24,'behaviors':[{'id':6002714895372,'name':'All travelers'}],'genders':[1],'geo_locations':{'countries':['US'],'regions':[{'key':'4081'}],'cities':[{'key':'777934','radius':10,'distance_unit':'mile'}]},'interests':[{'id':'<adsInterestID>','name':'<adsInterestName>'}],'life_events':[{'id':6002714398172,'name':'Newlywed (1 year)'}],'facebook_positions':['feed'],'publisher_platforms':['facebook','audience_network']},
   'status': 'PAUSED',
 }
```

### Comparing `facebook_business-9.0.2/examples/AdAccountAdSetsPostCreateAudienceNetwork.py` & `facebook_business-9.0.3/examples/AdAccountAdSetsPostCreateAudienceNetwork.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountAdSetsPostDailyBudget20.py` & `facebook_business-9.0.3/examples/AdAccountAdSetsPostDailyBudget20.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 FacebookAdsApi.init(access_token=access_token)
 
 fields = [
 ]
 params = {
   'name': 'My First Adset',
   'daily_budget': '2000',
-  'start_time': '2020-12-17T10:14:01-0800',
-  'end_time': '2020-12-24T10:14:01-0800',
+  'start_time': '2021-01-19T14:02:53-0800',
+  'end_time': '2021-01-26T14:02:53-0800',
   'campaign_id': '<adCampaignLinkClicksID>',
   'bid_amount': '100',
   'billing_event': 'LINK_CLICKS',
   'optimization_goal': 'LINK_CLICKS',
   'targeting': {'facebook_positions':['feed'],'geo_locations':{'countries':['US']}},
   'status': 'PAUSED',
 }
```

### Comparing `facebook_business-9.0.2/examples/AdAccountAdSetsPostDemographicTargeting.py` & `facebook_business-9.0.3/examples/AdAccountAdSetsPostDemographicTargeting.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountAdSetsPostInterestTargeting.py` & `facebook_business-9.0.3/examples/AdAccountAdSetsPostInterestTargeting.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountAdSetsPostLifetimeBudget200Duration10Days.py` & `facebook_business-9.0.3/examples/AdAccountAdSetsPostLifetimeBudget200Duration10Days.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 FacebookAdsApi.init(access_token=access_token)
 
 fields = [
 ]
 params = {
   'name': 'My First Adset',
   'lifetime_budget': '20000',
-  'start_time': '2020-12-17T10:14:10-0800',
-  'end_time': '2020-12-27T10:14:10-0800',
+  'start_time': '2021-01-19T14:03:02-0800',
+  'end_time': '2021-01-29T14:03:02-0800',
   'campaign_id': '<adCampaignLinkClicksID>',
   'bid_amount': '100',
   'billing_event': 'LINK_CLICKS',
   'optimization_goal': 'LINK_CLICKS',
   'targeting': {'facebook_positions':['feed'],'geo_locations':{'countries':['US']},'publisher_platforms':['facebook','audience_network']},
   'status': 'PAUSED',
 }
```

### Comparing `facebook_business-9.0.2/examples/AdAccountAdSetsPostOfferClaim.py` & `facebook_business-9.0.3/examples/AdAccountAdSetsPostReach.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,22 +27,21 @@
 app_id = '<APP_ID>'
 id = '<AD_ACCOUNT_ID>'
 FacebookAdsApi.init(access_token=access_token)
 
 fields = [
 ]
 params = {
-  'name': 'My Offer Claim AdSet',
-  'lifetime_budget': '56000',
-  'start_time': '2020-12-17T10:13:52-0800',
-  'end_time': '2020-12-24T10:13:52-0800',
+  'name': 'My Reach Ad Set',
+  'optimization_goal': 'REACH',
+  'billing_event': 'IMPRESSIONS',
+  'bid_amount': '2',
+  'daily_budget': '1000',
   'campaign_id': '<adCampaignLinkClicksID>',
-  'billing_event': 'LINK_CLICKS',
-  'optimization_goal': 'LINK_CLICKS',
-  'bid_amount': '1000',
-  'promoted_object': {'page_id':'<pageID>','offer_id':'<offerID>'},
-  'targeting': {'geo_locations':{'countries':['US']},'genders':[1],'age_min':'25','age_max':'55','facebook_positions':['feed']},
+  'targeting': {'excluded_geo_locations':{'regions':[{'key':'3847'}]},'geo_locations':{'countries':['US']},'facebook_positions':['feed']},
+  'status': 'PAUSED',
+  'promoted_object': {'page_id':'<pageID>'},
 }
 print AdAccount(id).create_ad_set(
   fields=fields,
   params=params,
 )
```

### Comparing `facebook_business-9.0.2/examples/AdAccountAdSetsPostOptimizePostEngagement.py` & `facebook_business-9.0.3/examples/AdAccountAdSetsPostPlacementTargeting.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,22 +27,20 @@
 app_id = '<APP_ID>'
 id = '<AD_ACCOUNT_ID>'
 FacebookAdsApi.init(access_token=access_token)
 
 fields = [
 ]
 params = {
-  'name': 'My First Adset',
-  'lifetime_budget': '20000',
-  'start_time': '2020-12-17T10:14:20-0800',
-  'end_time': '2020-12-27T10:14:20-0800',
-  'campaign_id': '<adCampaignLinkClicksID>',
-  'bid_amount': '500',
+  'name': 'My AdSet',
+  'optimization_goal': 'REACH',
   'billing_event': 'IMPRESSIONS',
-  'optimization_goal': 'POST_ENGAGEMENT',
-  'targeting': {'facebook_positions':['feed'],'geo_locations':{'countries':['US'],'regions':[{'key':'4081'}],'cities':[{'key':777934,'radius':10,'distance_unit':'mile'}]},'genders':[1],'age_max':24,'age_min':20,'behaviors':[{'id':6002714895372,'name':'All travelers'}],'life_events':[{'id':6002714398172,'name':'Newlywed (1 year)'}],'publisher_platforms':['facebook'],'device_platforms':['desktop']},
-  'status': 'PAUSED',
+  'bid_amount': '2',
+  'daily_budget': '1000',
+  'campaign_id': '<adCampaignLinkClicksID>',
+  'targeting': {'geo_locations':{'countries':['US']},'publisher_platforms':['facebook'],'facebook_positions':['feed']},
+  'promoted_object': {'page_id':'<pageID>'},
 }
 print AdAccount(id).create_ad_set(
   fields=fields,
   params=params,
 )
```

### Comparing `facebook_business-9.0.2/examples/AdAccountAdSetsPostPageLikes.py` & `facebook_business-9.0.3/examples/AdAccountAdSetsPostPageLikes.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountAdSetsPostPlacementTargeting.py` & `facebook_business-9.0.3/examples/AdAccountAdSetsPostOfferClaim.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,20 +27,22 @@
 app_id = '<APP_ID>'
 id = '<AD_ACCOUNT_ID>'
 FacebookAdsApi.init(access_token=access_token)
 
 fields = [
 ]
 params = {
-  'name': 'My AdSet',
-  'optimization_goal': 'REACH',
-  'billing_event': 'IMPRESSIONS',
-  'bid_amount': '2',
-  'daily_budget': '1000',
+  'name': 'My Offer Claim AdSet',
+  'lifetime_budget': '56000',
+  'start_time': '2021-01-19T14:02:43-0800',
+  'end_time': '2021-01-26T14:02:43-0800',
   'campaign_id': '<adCampaignLinkClicksID>',
-  'targeting': {'geo_locations':{'countries':['US']},'publisher_platforms':['facebook'],'facebook_positions':['feed']},
-  'promoted_object': {'page_id':'<pageID>'},
+  'billing_event': 'LINK_CLICKS',
+  'optimization_goal': 'LINK_CLICKS',
+  'bid_amount': '1000',
+  'promoted_object': {'page_id':'<pageID>','offer_id':'<offerID>'},
+  'targeting': {'geo_locations':{'countries':['US']},'genders':[1],'age_min':'25','age_max':'55','facebook_positions':['feed']},
 }
 print AdAccount(id).create_ad_set(
   fields=fields,
   params=params,
 )
```

### Comparing `facebook_business-9.0.2/examples/AdAccountAdSetsPostReach.py` & `facebook_business-9.0.3/examples/AdAccountGeneratePreviewsEdgeMaiaWithObjectStorySpec.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,33 +15,26 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 from facebook_business.adobjects.adaccount import AdAccount
-from facebook_business.adobjects.adset import AdSet
+from facebook_business.adobjects.adpreview import AdPreview
 from facebook_business.api import FacebookAdsApi
 
 access_token = '<ACCESS_TOKEN>'
 app_secret = '<APP_SECRET>'
 app_id = '<APP_ID>'
 id = '<AD_ACCOUNT_ID>'
 FacebookAdsApi.init(access_token=access_token)
 
 fields = [
 ]
 params = {
-  'name': 'My Reach Ad Set',
-  'optimization_goal': 'REACH',
-  'billing_event': 'IMPRESSIONS',
-  'bid_amount': '2',
-  'daily_budget': '1000',
-  'campaign_id': '<adCampaignLinkClicksID>',
-  'targeting': {'excluded_geo_locations':{'regions':[{'key':'3847'}]},'geo_locations':{'countries':['US']},'facebook_positions':['feed']},
-  'status': 'PAUSED',
-  'promoted_object': {'page_id':'<pageID>'},
+  'creative': {'object_story_spec':{'link_data':{'call_to_action':{'type':'USE_APP','value':{'link':'<url>'}},'description':'Description','link':'<url>','message':'Message','name':'Name','picture':'<imageURL>'},'page_id':'<pageID>'}},
+  'ad_format': 'MOBILE_FEED_STANDARD',
 }
-print AdAccount(id).create_ad_set(
+print AdAccount(id).get_generate_previews(
   fields=fields,
   params=params,
 )
```

### Comparing `facebook_business-9.0.2/examples/AdAccountAdVideosPost.py` & `facebook_business-9.0.3/examples/AdAccountAdVideosPost.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountAdsPixelEdgeGetPixelCode.py` & `facebook_business-9.0.3/examples/AdAccountAdsPixelEdgeGetPixelCode.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountAdsPixelsPost.py` & `facebook_business-9.0.3/examples/AdAccountAdsPixelsPost.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountAdsPost.py` & `facebook_business-9.0.3/examples/AdAccountAdsPost.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountAdsPostAdsRedownload.py` & `facebook_business-9.0.3/examples/AdAccountAdsPostAdsRedownload.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountAdsPostOfferClaim.py` & `facebook_business-9.0.3/examples/AdAccountAdsPostOfferClaim.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountAdsPostTrackingPostEngagement.py` & `facebook_business-9.0.3/examples/AdAccountAdsPostTrackingPostEngagement.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountCampaignsEdge.py` & `facebook_business-9.0.3/examples/AdAccountCampaignsEdge.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountCampaignsPostConversions.py` & `facebook_business-9.0.3/examples/AdAccountCampaignsPostConversions.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountCampaignsPostEventResponses.py` & `facebook_business-9.0.3/examples/AdAccountCampaignsPostEventResponses.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountCampaignsPostLeadGen.py` & `facebook_business-9.0.3/examples/AdAccountCampaignsPostLeadGen.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountCampaignsPostLinkClicks.py` & `facebook_business-9.0.3/examples/AdAccountCampaignsPostLinkClicks.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountCampaignsPostLocalAwareness.py` & `facebook_business-9.0.3/examples/AdAccountCampaignsPostLocalAwareness.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountCampaignsPostMAIA.py` & `facebook_business-9.0.3/examples/AdAccountCampaignsPostMAIA.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountCampaignsPostMAIDPA.py` & `facebook_business-9.0.3/examples/AdAccountCampaignsPostMAIDPA.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountCampaignsPostOfferClaims.py` & `facebook_business-9.0.3/examples/AdAccountCampaignsPostOfferClaims.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountCampaignsPostPageLikes.py` & `facebook_business-9.0.3/examples/AdAccountCampaignsPostPageLikes.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountCampaignsPostPostEngagement.py` & `facebook_business-9.0.3/examples/AdAccountCampaignsPostPostEngagement.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountCampaignsPostStoreCampaign.py` & `facebook_business-9.0.3/examples/AdAccountCampaignsPostStoreCampaign.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountCampaignsPostVideoViews.py` & `facebook_business-9.0.3/examples/AdAccountCampaignsPostVideoViews.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountCustomAudiencesEdge.py` & `facebook_business-9.0.3/examples/AdAccountCustomAudiencesEdge.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountCustomAudiencesEdgeDataSourceSubtype.py` & `facebook_business-9.0.3/examples/AdAccountCustomAudiencesEdgeDataSourceSubtype.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountCustomAudiencesPostCreateCustomAudience.py` & `facebook_business-9.0.3/examples/AdAccountCustomAudiencesPostCreateCustomAudience.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountCustomAudiencesPostDynamicEventValueBasedLookalikeCustomAudience.py` & `facebook_business-9.0.3/examples/AdAccountCustomAudiencesPostDynamicEventValueBasedLookalikeCustomAudience.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountCustomAudiencesPostDynamicValueBasedLookalikeCustomAudience.py` & `facebook_business-9.0.3/examples/AdAccountCustomAudiencesPostDynamicValueBasedLookalikeCustomAudience.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountCustomAudiencesPostPlatformCustomAudienceMACARule.py` & `facebook_business-9.0.3/examples/AdAccountCustomAudiencesPostPlatformCustomAudienceMACARule.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountCustomAudiencesPostPlatformECAExclusions.py` & `facebook_business-9.0.3/examples/AdAccountCustomAudiencesPostPlatformECAExclusions.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountCustomAudiencesPostPlatformECAMultiFilters.py` & `facebook_business-9.0.3/examples/AdAccountCustomAudiencesPostPlatformECAMultiFilters.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountCustomAudiencesPostPlatformECAMultiPages.py` & `facebook_business-9.0.3/examples/AdAccountCustomAudiencesPostPlatformECAMultiPages.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountCustomAudiencesPostPlatformEngagementCustomAudience.py` & `facebook_business-9.0.3/examples/AdAccountCustomAudiencesPostPlatformEngagementCustomAudience.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountCustomAudiencesPostPlatformWebsiteCustomAudience.py` & `facebook_business-9.0.3/examples/AdAccountCustomAudiencesPostPlatformWebsiteCustomAudience.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountCustomAudiencesPostValueBasedCustomAudience.py` & `facebook_business-9.0.3/examples/AdAccountCustomAudiencesPostValueBasedCustomAudience.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountCustomAudiencesPostValueBasedLookalikeCustomAudience.py` & `facebook_business-9.0.3/examples/AdAccountCustomAudiencesPostValueBasedLookalikeCustomAudience.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountGeneratePreviewsEdge.py` & `facebook_business-9.0.3/examples/AdAccountGeneratePreviewsEdge.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountGeneratePreviewsEdgeDesktopWithStoryId.py` & `facebook_business-9.0.3/examples/AdAccountGeneratePreviewsEdgeDesktopWithStoryId.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountGeneratePreviewsEdgeInstagramStandards.py` & `facebook_business-9.0.3/examples/AdAccountGeneratePreviewsEdgeInstagramStandards.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountGeneratePreviewsEdgeMaiaWithObjectStorySpec.py` & `facebook_business-9.0.3/examples/CustomAudienceUsersPost.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,27 +14,25 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
-from facebook_business.adobjects.adaccount import AdAccount
-from facebook_business.adobjects.adpreview import AdPreview
+from facebook_business.adobjects.customaudience import CustomAudience
 from facebook_business.api import FacebookAdsApi
 
 access_token = '<ACCESS_TOKEN>'
 app_secret = '<APP_SECRET>'
 app_id = '<APP_ID>'
-id = '<AD_ACCOUNT_ID>'
+id = '<CUSTOM_AUDIENCE_ID>'
 FacebookAdsApi.init(access_token=access_token)
 
 fields = [
 ]
 params = {
-  'creative': {'object_story_spec':{'link_data':{'call_to_action':{'type':'USE_APP','value':{'link':'<url>'}},'description':'Description','link':'<url>','message':'Message','name':'Name','picture':'<imageURL>'},'page_id':'<pageID>'}},
-  'ad_format': 'MOBILE_FEED_STANDARD',
+  'payload': {'schema':['EMAIL','LOOKALIKE_VALUE'],'data':[['9b431636bd164765d63c573c346708846af4f68fe3701a77a3bdd7e7e5166254',44.5],['8cc62c145cd0c6dc444168eaeb1b61b351f9b1809a579cc9b4c9e9d7213a39ee',140],['4eaf70b1f7a797962b9d2a533f122c8039012b31e0a52b34a426729319cb792a',0],['98df8d46f118f8bef552b0ec0a3d729466a912577830212a844b73960777ac56',0.9]]},
 }
-print AdAccount(id).get_generate_previews(
+print CustomAudience(id).create_user(
   fields=fields,
   params=params,
 )
```

### Comparing `facebook_business-9.0.2/examples/AdAccountNode.py` & `facebook_business-9.0.3/examples/AdAccountNode.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountProductAudiencesPostIphoneViewNoPurchase.py` & `facebook_business-9.0.3/examples/AdAccountProductAudiencesPostIphoneViewNoPurchase.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountProductAudiencesPostNoPurchase.py` & `facebook_business-9.0.3/examples/AdAccountProductAudiencesPostNoPurchase.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdAccountReachEstimate.py` & `facebook_business-9.0.3/examples/AdAccountReachEstimate.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdCampaignActivityNode.py` & `facebook_business-9.0.3/examples/AdCampaignActivityNode.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdCampaignGroupActivityNode.py` & `facebook_business-9.0.3/examples/AdCampaignGroupActivityNode.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdCampaignGroupAdsEdge.py` & `facebook_business-9.0.3/examples/AdCampaignGroupAdsEdge.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdCampaignGroupAdsEdgeAdgroupsWithStatusArchived.py` & `facebook_business-9.0.3/examples/AdCampaignGroupAdsEdgeAdgroupsWithStatusArchived.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdCampaignGroupAdsetsEdge.py` & `facebook_business-9.0.3/examples/AdCampaignGroupAdsetsEdge.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdCampaignNode.py` & `facebook_business-9.0.3/examples/AdCampaignNode.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdCampaignPost.py` & `facebook_business-9.0.3/examples/AdCampaignPost.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdCampaignPostAdsetUpdateCpa.py` & `facebook_business-9.0.3/examples/AdCampaignPostAdsetUpdateCpa.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdCreativeCreativeInsightsEdge.py` & `facebook_business-9.0.3/examples/AdCreativeCreativeInsightsEdge.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdCreativeNode.py` & `facebook_business-9.0.3/examples/AdCreativeNode.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdCreativeNodeRead.py` & `facebook_business-9.0.3/examples/AdCreativeNodeRead.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdCreativeNodeReadInstagramPermalinkUrl.py` & `facebook_business-9.0.3/examples/AdCreativeNodeReadInstagramPermalinkUrl.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdCreativePreviewsEdge.py` & `facebook_business-9.0.3/examples/AdCreativePreviewsEdge.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdCreativePreviewsEdgePreview.py` & `facebook_business-9.0.3/examples/AdCreativePreviewsEdgePreview.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdCreativePreviewsEdgePreviewDynamicAds.py` & `facebook_business-9.0.3/examples/AdCreativePreviewsEdgePreviewDynamicAds.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdCreativePreviewsEdgePreviewDynamicAdsWithCustomizations.py` & `facebook_business-9.0.3/examples/AdCreativePreviewsEdgePreviewDynamicAdsWithCustomizations.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdgroupActivityNode.py` & `facebook_business-9.0.3/examples/AdgroupActivityNode.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdgroupLeadsEdgeAdgroupLeads.py` & `facebook_business-9.0.3/examples/AdgroupLeadsEdgeAdgroupLeads.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdgroupLeadsEdgeAdgroupLeadsDPA.py` & `facebook_business-9.0.3/examples/AdgroupLeadsEdgeAdgroupLeadsDPA.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdgroupLeadsEdgeAdgroupLeadsFiltered.py` & `facebook_business-9.0.3/examples/AdgroupLeadsEdgeAdgroupLeadsFiltered.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,13 +27,13 @@
 app_id = '<APP_ID>'
 id = '<AD_GROUP_ID>'
 FacebookAdsApi.init(access_token=access_token)
 
 fields = [
 ]
 params = {
-  'filtering': [{'field':'time_created','operator':'GREATER_THAN','value':1607393319}],
+  'filtering': [{'field':'time_created','operator':'GREATER_THAN','value':1610489349}],
 }
 print Ad(id).get_leads(
   fields=fields,
   params=params,
 )
```

### Comparing `facebook_business-9.0.2/examples/AdgroupPost.py` & `facebook_business-9.0.3/examples/AdgroupPost.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdgroupPostUpdateStatus.py` & `facebook_business-9.0.3/examples/AdgroupPostUpdateStatus.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdsInsightsEdgeAdCampaignInsights.py` & `facebook_business-9.0.3/examples/AdsInsightsEdgeAdCampaignInsights.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdsInsightsEdgeStoreVisitsAdCampaignInsights.py` & `facebook_business-9.0.3/examples/AdsInsightsEdgeStoreVisitsAdCampaignInsights.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdsPixelEventsPost.py` & `facebook_business-9.0.3/examples/AdsPixelEventsPost.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,13 +26,13 @@
 app_id = '<APP_ID>'
 id = '<ADS_PIXEL_ID>'
 FacebookAdsApi.init(access_token=access_token)
 
 fields = [
 ]
 params = {
-  'data': [{'event_name':'PageView','event_time':1607998596,'user_data':{'fbc':'fb.1.1554763741205.AbCdEfGhIjKlMnOpQrStUvWxYz1234567890','fbp':'fb.1.1558571054389.1098115397','em':'309a0a5c3e211326ae75ca18196d301a9bdbd1a882a4d2569511033da23f0abd'}}],
+  'data': [{'event_name':'PageView','event_time':1610578702,'user_data':{'fbc':'fb.1.1554763741205.AbCdEfGhIjKlMnOpQrStUvWxYz1234567890','fbp':'fb.1.1558571054389.1098115397','em':'309a0a5c3e211326ae75ca18196d301a9bdbd1a882a4d2569511033da23f0abd'}}],
 }
 print AdsPixel(id).create_event(
   fields=fields,
   params=params,
 )
```

### Comparing `facebook_business-9.0.2/examples/AdsPixelEventsPostCustom.py` & `facebook_business-9.0.3/examples/AdsPixelEventsPostCustom.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,44 +16,51 @@
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import time
 
+from facebook_business.adobjects.serverside.action_source import ActionSource
+from facebook_business.adobjects.serverside.custom_data import CustomData
 from facebook_business.adobjects.serverside.event import Event
 from facebook_business.adobjects.serverside.event_request import EventRequest
 from facebook_business.adobjects.serverside.user_data import UserData
-from facebook_business.adobjects.serverside.custom_data import CustomData
 from facebook_business.api import FacebookAdsApi
 
 access_token = '<ACCESS_TOKEN>'
 pixel_id = 'ADS_PIXEL_ID>'
 
 FacebookAdsApi.init(access_token=access_token)
 
 user_data = UserData(
     email='joe@eg.com',
+    # It is recommended to send Client IP and User Agent for Conversions API Events.
+    client_ip_address=request.META.get('REMOTE_ADDR'),
+    client_user_agent=request.headers['User-Agent'],
     fbc='fb.1.1554763741205.AbCdEfGhIjKlMnOpQrStUvWxYz1234567890',
-    fbp='fb.1.1558571054389.1098115397'
+    fbp='fb.1.1558571054389.1098115397',
 )
 
 custom_data = CustomData(
     currency='usd',
-    value=123.45
+    value=123.45,
 )
 
 event = Event(
     event_name='Purchase',
     event_time=int(time.time()),
     user_data=user_data,
     custom_data=custom_data,
+    event_source_url='http://jaspers-market.com/product/123',
+    action_source=ActionSource.WEBSITE,
 )
 
 events = [event]
 
 event_request = EventRequest(
     events=events,
-    pixel_id=pixel_id)
+    pixel_id=pixel_id,
+)
 
 event_response = event_request.execute()
 print(event_response)
```

### Comparing `facebook_business-9.0.2/examples/AdsPixelSharedAccountsEdge.py` & `facebook_business-9.0.3/examples/AdsPixelSharedAccountsEdge.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdsPixelSharedAccountsPost.py` & `facebook_business-9.0.3/examples/AdsPixelSharedAccountsPost.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/AdsPixelSharedAgenciesEdge.py` & `facebook_business-9.0.3/examples/AdsPixelSharedAgenciesEdge.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/BusinessOwnedProductCatalogsPostDestinationCatalog.py` & `facebook_business-9.0.3/examples/BusinessOwnedProductCatalogsPostDestinationCatalog.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/BusinessOwnedProductCatalogsPostFlightCatalog.py` & `facebook_business-9.0.3/examples/BusinessOwnedProductCatalogsPostFlightCatalog.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/BusinessOwnedProductCatalogsPostHotelCatalog.py` & `facebook_business-9.0.3/examples/BusinessOwnedProductCatalogsPostHotelCatalog.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/BusinessOwnedProductCatalogsPostProductCatalog.py` & `facebook_business-9.0.3/examples/BusinessOwnedProductCatalogsPostProductCatalog.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/CustomAudienceDelete.py` & `facebook_business-9.0.3/examples/CustomAudienceDelete.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/CustomAudienceNode.py` & `facebook_business-9.0.3/examples/CustomAudienceNode.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/CustomAudienceNodeReadRule.py` & `facebook_business-9.0.3/examples/CustomAudienceNodeReadRule.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/CustomAudiencePost.py` & `facebook_business-9.0.3/examples/CustomAudiencePost.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/CustomAudienceUsersPost.py` & `facebook_business-9.0.3/examples/CustomAudienceUsersPostCrossPlatform.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,13 +26,13 @@
 app_id = '<APP_ID>'
 id = '<CUSTOM_AUDIENCE_ID>'
 FacebookAdsApi.init(access_token=access_token)
 
 fields = [
 ]
 params = {
-  'payload': {'schema':['EMAIL','LOOKALIKE_VALUE'],'data':[['9b431636bd164765d63c573c346708846af4f68fe3701a77a3bdd7e7e5166254',44.5],['8cc62c145cd0c6dc444168eaeb1b61b351f9b1809a579cc9b4c9e9d7213a39ee',140],['4eaf70b1f7a797962b9d2a533f122c8039012b31e0a52b34a426729319cb792a',0],['98df8d46f118f8bef552b0ec0a3d729466a912577830212a844b73960777ac56',0.9]]},
+  'payload': {'schema':['EMAIL','MADID','APPUID','LOOKALIKE_VALUE'],'app_ids':['<appID>'],'data':[['b36a83701f1c3191e19722d6f90274bc1b5501fe69ebf33313e440fe4b0fe210','6032d997-3ab0-4de0-aa16-8af0e5b482fb','1234567890','0.9'],['2b3b2b9ce842ab8b6a6c614cb1f9604bb8a0d502d1af49c526b72b10894e95b5','B67385F8-9A82-4670-8C0A-6F9EA7513F5F','','0'],['898628e28890f937bdf009391def42879c401a4bcf1b5fd24e738d9f5da8cbbb','','9876543210','0.4']]},
 }
 print CustomAudience(id).create_user(
   fields=fields,
   params=params,
 )
```

### Comparing `facebook_business-9.0.2/examples/CustomAudienceUsersPostCrossPlatform.py` & `facebook_business-9.0.3/facebook_business/adobjects/adbidadjustments.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,25 +14,42 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
-from facebook_business.adobjects.customaudience import CustomAudience
-from facebook_business.api import FacebookAdsApi
+from facebook_business.adobjects.abstractobject import AbstractObject
+
+"""
+This class is auto-generated.
+
+For any issues or feature requests related to this class, please let us know on
+github and we'll fix in our codegen framework. We'll not be able to accept
+pull request for this class.
+"""
+
+class AdBidAdjustments(
+    AbstractObject,
+):
+
+    def __init__(self, api=None):
+        super(AdBidAdjustments, self).__init__()
+        self._isAdBidAdjustments = True
+        self._api = api
+
+    class Field(AbstractObject.Field):
+        age_range = 'age_range'
+        page_types = 'page_types'
+        user_groups = 'user_groups'
+
+    _field_types = {
+        'age_range': 'map<string, float>',
+        'page_types': 'Object',
+        'user_groups': 'string',
+    }
+    @classmethod
+    def _get_field_enum_info(cls):
+        field_enum_info = {}
+        return field_enum_info
+
 
-access_token = '<ACCESS_TOKEN>'
-app_secret = '<APP_SECRET>'
-app_id = '<APP_ID>'
-id = '<CUSTOM_AUDIENCE_ID>'
-FacebookAdsApi.init(access_token=access_token)
-
-fields = [
-]
-params = {
-  'payload': {'schema':['EMAIL','MADID','APPUID','LOOKALIKE_VALUE'],'app_ids':['<appID>'],'data':[['b36a83701f1c3191e19722d6f90274bc1b5501fe69ebf33313e440fe4b0fe210','6032d997-3ab0-4de0-aa16-8af0e5b482fb','1234567890','0.9'],['2b3b2b9ce842ab8b6a6c614cb1f9604bb8a0d502d1af49c526b72b10894e95b5','B67385F8-9A82-4670-8C0A-6F9EA7513F5F','','0'],['898628e28890f937bdf009391def42879c401a4bcf1b5fd24e738d9f5da8cbbb','','9876543210','0.4']]},
-}
-print CustomAudience(id).create_user(
-  fields=fields,
-  params=params,
-)
```

### Comparing `facebook_business-9.0.2/examples/MultiPageFeedCreateThenDelete.py` & `facebook_business-9.0.3/examples/MultiPageFeedCreateThenDelete.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/MultiPromoteYourPage.py` & `facebook_business-9.0.3/examples/MultiPromoteYourPage.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/OfflineConversionsCreateOfflineSet.py` & `facebook_business-9.0.3/examples/OfflineConversionsCreateOfflineSet.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/PageFeedEdge.py` & `facebook_business-9.0.3/examples/PageFeedEdge.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/PageFeedPost.py` & `facebook_business-9.0.3/examples/PageFeedPost.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/PageFeedPostFeedImageDeepLink.py` & `facebook_business-9.0.3/examples/PageFeedPostFeedImageDeepLink.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/PageNode.py` & `facebook_business-9.0.3/examples/PageNode.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/PageNodePageSearch.py` & `facebook_business-9.0.3/examples/PageNodePageSearch.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/PagePhotosEdge.py` & `facebook_business-9.0.3/examples/PagePhotosEdge.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/PagePhotosPost.py` & `facebook_business-9.0.3/examples/PagePhotosPost.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/PagePictureEdge.py` & `facebook_business-9.0.3/examples/PagePictureEdge.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/PagePostCommentsEdge.py` & `facebook_business-9.0.3/examples/PagePostCommentsEdge.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/PagePostCommentsPost.py` & `facebook_business-9.0.3/examples/PagePostCommentsPost.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/PagePostDelete.py` & `facebook_business-9.0.3/examples/PagePostDelete.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/PagePostNode.py` & `facebook_business-9.0.3/examples/PagePostNode.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/PagePostPost.py` & `facebook_business-9.0.3/examples/PagePostPost.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/PagePostsEdge.py` & `facebook_business-9.0.3/examples/PagePostsEdge.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/PagePostsEdgePagePostCreateCarousel.py` & `facebook_business-9.0.3/examples/PagePostsEdgePagePostCreateCarousel.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/PageRolesEdge.py` & `facebook_business-9.0.3/examples/PageRolesEdge.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/PageSubscribedAppsPost.py` & `facebook_business-9.0.3/examples/PageSubscribedAppsPost.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/ProductCatalogEventStatsEdge.py` & `facebook_business-9.0.3/examples/ProductCatalogEventStatsEdge.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/ProductCatalogHotelsPost.py` & `facebook_business-9.0.3/examples/ProductCatalogHotelsPost.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/ProductCatalogHotelsPostUpdateHotelsCatalogSettings.py` & `facebook_business-9.0.3/examples/ProductCatalogHotelsPostUpdateHotelsCatalogSettings.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/ProductCatalogProductFeedsPostProductFeed.py` & `facebook_business-9.0.3/examples/ProductCatalogProductFeedsPostProductFeed.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/ProductCatalogProductSetsPostHotelSet.py` & `facebook_business-9.0.3/examples/ProductCatalogProductSetsPostHotelSet.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/ProductCatalogProductSetsPostProductSet.py` & `facebook_business-9.0.3/examples/ProductCatalogProductSetsPostProductSet.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/ServerSideApi.py` & `facebook_business-9.0.3/examples/ServerSideApi.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/UserAccountsEdge.py` & `facebook_business-9.0.3/examples/UserAccountsEdge.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/UserAdAccountsEdge.py` & `facebook_business-9.0.3/examples/UserAdAccountsEdge.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/UserLeadGenInfoNode.py` & `facebook_business-9.0.3/examples/UserLeadGenInfoNode.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/UserNode.py` & `facebook_business-9.0.3/examples/UserNode.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/VideoThumbnailsEdge.py` & `facebook_business-9.0.3/examples/VideoThumbnailsEdge.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/ad_creation_utils.py` & `facebook_business-9.0.3/examples/ad_creation_utils.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/async.py` & `facebook_business-9.0.3/examples/async.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/batch_create.py` & `facebook_business-9.0.3/examples/batch_create.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/batch_pause.py` & `facebook_business-9.0.3/examples/batch_pause.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/batch_utils.py` & `facebook_business-9.0.3/examples/batch_utils.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/custom_audience_utils.py` & `facebook_business-9.0.3/examples/custom_audience_utils.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/dpa-update/dpa_search.py` & `facebook_business-9.0.3/examples/dpa-update/dpa_search.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/dpa-update/dpa_update.py` & `facebook_business-9.0.3/examples/dpa-update/dpa_update.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/dpa-update/stock_update.py` & `facebook_business-9.0.3/examples/dpa-update/stock_update.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/my_app_session.cfg.dist` & `facebook_business-9.0.3/examples/my_app_session.cfg.dist`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/read_objects.py` & `facebook_business-9.0.3/examples/read_objects.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/simple_create.py` & `facebook_business-9.0.3/examples/simple_create.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/test.png` & `facebook_business-9.0.3/examples/test.png`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/examples/upload_video.py` & `facebook_business-9.0.3/examples/upload_video.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/__init__.py` & `facebook_business-9.0.3/facebook_business/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,13 +17,13 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 from facebook_business.session import FacebookSession
 from facebook_business.api import FacebookAdsApi
 
-__version__ = '9.0.2'
+__version__ = '9.0.3'
 __all__ = [
     'session',
     'objects',
     'api',
 ]
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/__init__.py` & `facebook_business-9.0.3/facebook_business/adobjects/__init__.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/abstractcrudobject.py` & `facebook_business-9.0.3/facebook_business/adobjects/abstractcrudobject.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/abstractobject.py` & `facebook_business-9.0.3/facebook_business/adobjects/abstractobject.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/ad.py` & `facebook_business-9.0.3/facebook_business/adobjects/ad.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adaccount.py` & `facebook_business-9.0.3/facebook_business/adobjects/adaccount.py`

 * *Files 0% similar despite different names*

```diff
@@ -545,14 +545,15 @@
             'messenger_sponsored_message': 'string',
             'name': 'string',
             'object_id': 'unsigned int',
             'object_story_id': 'string',
             'object_story_spec': 'AdCreativeObjectStorySpec',
             'object_type': 'string',
             'object_url': 'string',
+            'place_page_set_id': 'string',
             'platform_customizations': 'Object',
             'playable_asset_id': 'string',
             'portrait_customizations': 'map',
             'product_set_id': 'string',
             'recommender_settings': 'map',
             'source_instagram_media_id': 'string',
             'template_url': 'string',
@@ -1455,15 +1456,14 @@
           api_utils.warning('`success` and `failure` callback only work for batch call.')
         from facebook_business.adobjects.advideo import AdVideo
         param_types = {
             'adaptive_type': 'string',
             'animated_effect_id': 'unsigned int',
             'application_id': 'string',
             'asked_fun_fact_prompt_id': 'unsigned int',
-            'attribution_app_id': 'string',
             'audio_story_wave_animation_handle': 'string',
             'chunk_session_id': 'string',
             'composer_entry_picker': 'string',
             'composer_entry_point': 'string',
             'composer_entry_time': 'unsigned int',
             'composer_session_events_log': 'string',
             'composer_session_id': 'string',
@@ -3318,49 +3318,14 @@
         )
         request.add_params(params)
         request.add_fields(fields)
 
         if batch is not None:
             request.add_to_batch(batch, success=success, failure=failure)
             return request
-        elif pending:
-            return request
-        else:
-            self.assure_call()
-            return request.execute()
-
-    def get_roas(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
-        from facebook_business.utils import api_utils
-        if batch is None and (success is not None or failure is not None):
-          api_utils.warning('`success` and `failure` callback only work for batch call.')
-        from facebook_business.adobjects.adaccountroas import AdAccountRoas
-        param_types = {
-            'fields': 'list<string>',
-            'filtering': 'list<Object>',
-            'time_increment': 'string',
-            'time_range': 'Object',
-        }
-        enums = {
-        }
-        request = FacebookRequest(
-            node_id=self['id'],
-            method='GET',
-            endpoint='/roas',
-            api=self._api,
-            param_checker=TypeChecker(param_types, enums),
-            target_class=AdAccountRoas,
-            api_type='EDGE',
-            response_parser=ObjectParser(target_class=AdAccountRoas, api=self._api),
-        )
-        request.add_params(params)
-        request.add_fields(fields)
-
-        if batch is not None:
-            request.add_to_batch(batch, success=success, failure=failure)
-            return request
         elif pending:
             return request
         else:
             self.assure_call()
             return request.execute()
 
     def get_saved_audiences(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adaccountactivity.py` & `facebook_business-9.0.3/facebook_business/adobjects/adaccountactivity.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adaccountadruleshistory.py` & `facebook_business-9.0.3/facebook_business/adobjects/adaccountadruleshistory.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adaccountadvolume.py` & `facebook_business-9.0.3/facebook_business/adobjects/adaccountadvolume.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adaccountcontentfilterlevelsinheritance.py` & `facebook_business-9.0.3/facebook_business/adobjects/adaccountcontentfilterlevelsinheritance.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adaccountdefaultdestination.py` & `facebook_business-9.0.3/facebook_business/adobjects/adaccountdefaultdestination.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adaccountdefaultobjective.py` & `facebook_business-9.0.3/facebook_business/adobjects/adaccountdefaultobjective.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adaccountdeliveryestimate.py` & `facebook_business-9.0.3/facebook_business/adobjects/adaccountdeliveryestimate.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adaccountmatchedsearchapplicationsedgedata.py` & `facebook_business-9.0.3/facebook_business/adobjects/adaccountmatchedsearchapplicationsedgedata.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adaccountmaxbid.py` & `facebook_business-9.0.3/facebook_business/adobjects/adaccountmaxbid.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adaccountpromotableobjects.py` & `facebook_business-9.0.3/facebook_business/adobjects/adaccountpromotableobjects.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adaccountreachestimate.py` & `facebook_business-9.0.3/facebook_business/adobjects/adaccountreachestimate.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adaccountrecommendedcamapaignbudget.py` & `facebook_business-9.0.3/facebook_business/adobjects/adaccountrecommendedcamapaignbudget.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adaccountsubscribedapps.py` & `facebook_business-9.0.3/facebook_business/adobjects/adaccountsubscribedapps.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adaccounttargetingunified.py` & `facebook_business-9.0.3/facebook_business/adobjects/adaccounttargetingunified.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,15 +242,14 @@
         conversions = 'CONVERSIONS'
         event_responses = 'EVENT_RESPONSES'
         lead_generation = 'LEAD_GENERATION'
         link_clicks = 'LINK_CLICKS'
         local_awareness = 'LOCAL_AWARENESS'
         messages = 'MESSAGES'
         offer_claims = 'OFFER_CLAIMS'
-        outcome_leads = 'OUTCOME_LEADS'
         page_likes = 'PAGE_LIKES'
         post_engagement = 'POST_ENGAGEMENT'
         product_catalog_sales = 'PRODUCT_CATALOG_SALES'
         reach = 'REACH'
         store_visits = 'STORE_VISITS'
         video_views = 'VIDEO_VIEWS'
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adaccounttrackingdata.py` & `facebook_business-9.0.3/facebook_business/adobjects/adaccounttrackingdata.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adaccountuser.py` & `facebook_business-9.0.3/facebook_business/adobjects/adaccountuser.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adactivity.py` & `facebook_business-9.0.3/facebook_business/adobjects/adactivity.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adassetfeedspec.py` & `facebook_business-9.0.3/facebook_business/adobjects/adassetfeedspec.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         call_to_actions = 'call_to_actions'
         captions = 'captions'
         carousels = 'carousels'
         descriptions = 'descriptions'
         groups = 'groups'
         images = 'images'
         link_urls = 'link_urls'
+        onsite_destinations = 'onsite_destinations'
         optimization_type = 'optimization_type'
         posts = 'posts'
         titles = 'titles'
         videos = 'videos'
 
     class CallToActionTypes:
         add_to_cart = 'ADD_TO_CART'
@@ -132,14 +133,15 @@
         'call_to_actions': 'list<Object>',
         'captions': 'list<AdAssetFeedSpecCaption>',
         'carousels': 'list<Object>',
         'descriptions': 'list<AdAssetFeedSpecDescription>',
         'groups': 'list<AdAssetFeedSpecGroupRule>',
         'images': 'list<AdAssetFeedSpecImage>',
         'link_urls': 'list<AdAssetFeedSpecLinkURL>',
+        'onsite_destinations': 'list<Object>',
         'optimization_type': 'string',
         'posts': 'list<Object>',
         'titles': 'list<AdAssetFeedSpecTitle>',
         'videos': 'list<AdAssetFeedSpecVideo>',
     }
     @classmethod
     def _get_field_enum_info(cls):
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adassetfeedspecassetlabel.py` & `facebook_business-9.0.3/facebook_business/adobjects/adassetfeedspecassetlabel.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adassetfeedspecbody.py` & `facebook_business-9.0.3/facebook_business/adobjects/adassetfeedspecbody.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adassetfeedspeccaption.py` & `facebook_business-9.0.3/facebook_business/adobjects/adassetfeedspeccaption.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adassetfeedspecdescription.py` & `facebook_business-9.0.3/facebook_business/adobjects/adassetfeedspecdescription.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adassetfeedspecgrouprule.py` & `facebook_business-9.0.3/facebook_business/adobjects/adassetfeedspecgrouprule.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adassetfeedspecimage.py` & `facebook_business-9.0.3/facebook_business/adobjects/adassetfeedspecimage.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adassetfeedspeclinkurl.py` & `facebook_business-9.0.3/facebook_business/adobjects/adassetfeedspeclinkurl.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adassetfeedspectitle.py` & `facebook_business-9.0.3/facebook_business/adobjects/adassetfeedspectitle.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adassetfeedspecvideo.py` & `facebook_business-9.0.3/facebook_business/adobjects/adassetfeedspecvideo.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adasyncrequest.py` & `facebook_business-9.0.3/facebook_business/adobjects/adasyncrequest.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adasyncrequestset.py` & `facebook_business-9.0.3/facebook_business/adobjects/adasyncrequestset.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adasyncrequestsetnotificationresult.py` & `facebook_business-9.0.3/facebook_business/adobjects/adasyncrequestsetnotificationresult.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adbidadjustments.py` & `facebook_business-9.0.3/facebook_business/adobjects/richmediaelement.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,32 +24,32 @@
 This class is auto-generated.
 
 For any issues or feature requests related to this class, please let us know on
 github and we'll fix in our codegen framework. We'll not be able to accept
 pull request for this class.
 """
 
-class AdBidAdjustments(
+class RichMediaElement(
     AbstractObject,
 ):
 
     def __init__(self, api=None):
-        super(AdBidAdjustments, self).__init__()
-        self._isAdBidAdjustments = True
+        super(RichMediaElement, self).__init__()
+        self._isRichMediaElement = True
         self._api = api
 
     class Field(AbstractObject.Field):
-        age_range = 'age_range'
-        page_types = 'page_types'
-        user_groups = 'user_groups'
+        element = 'element'
+        element_type = 'element_type'
+        name = 'name'
 
     _field_types = {
-        'age_range': 'map<string, float>',
-        'page_types': 'Object',
-        'user_groups': 'string',
+        'element': 'Object',
+        'element_type': 'string',
+        'name': 'string',
     }
     @classmethod
     def _get_field_enum_info(cls):
         field_enum_info = {}
         return field_enum_info
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcampaignactivity.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcampaignactivity.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,29 +111,33 @@
         lowest_cost_with_bid_cap = 'LOWEST_COST_WITH_BID_CAP'
 
     class BillingEventNew:
         app_installs = 'APP_INSTALLS'
         clicks = 'CLICKS'
         impressions = 'IMPRESSIONS'
         link_clicks = 'LINK_CLICKS'
+        listing_interaction = 'LISTING_INTERACTION'
         none = 'NONE'
         offer_claims = 'OFFER_CLAIMS'
         page_likes = 'PAGE_LIKES'
         post_engagement = 'POST_ENGAGEMENT'
+        purchase = 'PURCHASE'
         thruplay = 'THRUPLAY'
 
     class BillingEventOld:
         app_installs = 'APP_INSTALLS'
         clicks = 'CLICKS'
         impressions = 'IMPRESSIONS'
         link_clicks = 'LINK_CLICKS'
+        listing_interaction = 'LISTING_INTERACTION'
         none = 'NONE'
         offer_claims = 'OFFER_CLAIMS'
         page_likes = 'PAGE_LIKES'
         post_engagement = 'POST_ENGAGEMENT'
+        purchase = 'PURCHASE'
         thruplay = 'THRUPLAY'
 
     class OptimizationGoalNew:
         ad_recall_lift = 'AD_RECALL_LIFT'
         app_downloads = 'APP_DOWNLOADS'
         app_installs = 'APP_INSTALLS'
         brand_awareness = 'BRAND_AWARENESS'
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcampaignbidconstraint.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcampaignbidconstraint.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcampaigndeliveryestimate.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcampaigndeliveryestimate.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcampaigndeliverystatsunsupportedreasons.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcampaigndeliverystatsunsupportedreasons.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcampaignfrequencycontrolspecs.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcampaignfrequencycontrolspecs.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcampaigngroupactivity.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcampaigngroupactivity.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcampaignissuesinfo.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcampaignissuesinfo.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcampaignlearningstageinfo.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcampaignlearningstageinfo.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcampaignoptimizationevent.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcampaignoptimizationevent.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcampaignpacedbidinfo.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcampaignpacedbidinfo.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcreative.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcreative.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcreativeaddisclaimer.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcreativeaddisclaimer.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcreativecollectionthumbnailinfo.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcreativecollectionthumbnailinfo.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcreativeinsights.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcreativeinsights.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcreativeinteractivecomponentsspec.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcreativeinteractivecomponentsspec.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcreativelinkdata.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcreativelinkdata.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcreativelinkdataapplinkspec.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcreativelinkdataapplinkspec.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcreativelinkdatacalltoaction.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcreativelinkdatacalltoaction.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcreativelinkdatacalltoactionvalue.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcreativelinkdatacalltoactionvalue.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcreativelinkdatachildattachment.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcreativelinkdatachildattachment.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcreativelinkdataimagelayerspec.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcreativelinkdataimagelayerspec.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcreativelinkdataimageoverlayspec.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcreativelinkdataimageoverlayspec.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcreativelinkdatasponsorshipinfospec.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcreativelinkdatasponsorshipinfospec.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcreativelinkdatatemplatevideospec.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcreativelinkdatatemplatevideospec.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcreativeobjectstoryspec.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcreativeobjectstoryspec.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcreativeomnichannellinkspec.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcreativeomnichannellinkspec.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcreativephotodata.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcreativephotodata.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcreativephotodatamediaelements.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcreativephotodatamediaelements.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcreativeplacedata.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcreativeplacedata.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcreativeplatformcustomization.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcreativeplatformcustomization.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcreativeportraitcustomizations.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcreativeportraitcustomizations.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcreativepostclickconfiguration.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcreativepostclickconfiguration.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcreativerecommendersettings.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcreativerecommendersettings.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcreativestaticfallbackspec.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcreativestaticfallbackspec.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcreativetemplateurlspec.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcreativetemplateurlspec.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcreativetextdata.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcreativetextdata.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcreativevideodata.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcreativevideodata.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adcustomizationrulespec.py` & `facebook_business-9.0.3/facebook_business/adobjects/adcustomizationrulespec.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/addynamiccreative.py` & `facebook_business-9.0.3/facebook_business/adobjects/addynamiccreative.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adentitytargetspend.py` & `facebook_business-9.0.3/facebook_business/adobjects/adentitytargetspend.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adgroupactivity.py` & `facebook_business-9.0.3/facebook_business/adobjects/adgroupactivity.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adgroupissuesinfo.py` & `facebook_business-9.0.3/facebook_business/adobjects/adgroupissuesinfo.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adgroupplacementspecificreviewfeedback.py` & `facebook_business-9.0.3/facebook_business/adobjects/adgroupplacementspecificreviewfeedback.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         dpa = 'dpa'
         dri_copyright = 'dri_copyright'
         dri_counterfeit = 'dri_counterfeit'
         facebook = 'facebook'
         facebook_pages_live_shopping = 'facebook_pages_live_shopping'
         instagram = 'instagram'
         instagram_shop = 'instagram_shop'
+        job_search = 'job_search'
         lead_gen_honeypot = 'lead_gen_honeypot'
         marketplace = 'marketplace'
         marketplace_home_rentals = 'marketplace_home_rentals'
         marketplace_home_sales = 'marketplace_home_sales'
         marketplace_motors = 'marketplace_motors'
         marketplace_shops = 'marketplace_shops'
         max_review_placements = 'max_review_placements'
@@ -85,14 +86,15 @@
         'dpa': 'map<string, string>',
         'dri_copyright': 'map<string, string>',
         'dri_counterfeit': 'map<string, string>',
         'facebook': 'map<string, string>',
         'facebook_pages_live_shopping': 'map<string, string>',
         'instagram': 'map<string, string>',
         'instagram_shop': 'map<string, string>',
+        'job_search': 'map<string, string>',
         'lead_gen_honeypot': 'map<string, string>',
         'marketplace': 'map<string, string>',
         'marketplace_home_rentals': 'map<string, string>',
         'marketplace_home_sales': 'map<string, string>',
         'marketplace_motors': 'map<string, string>',
         'marketplace_shops': 'map<string, string>',
         'max_review_placements': 'map<string, string>',
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adgrouprelevancescore.py` & `facebook_business-9.0.3/facebook_business/adobjects/adgrouprelevancescore.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adgroupreviewfeedback.py` & `facebook_business-9.0.3/facebook_business/adobjects/adgroupreviewfeedback.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adimage.py` & `facebook_business-9.0.3/facebook_business/adobjects/adimage.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adkeywords.py` & `facebook_business-9.0.3/facebook_business/adobjects/adkeywords.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adlabel.py` & `facebook_business-9.0.3/facebook_business/adobjects/adlabel.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/admonetizationproperty.py` & `facebook_business-9.0.3/facebook_business/adobjects/admonetizationproperty.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adnetworkanalyticsasyncqueryresult.py` & `facebook_business-9.0.3/facebook_business/adobjects/adnetworkanalyticsasyncqueryresult.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adnetworkanalyticssyncqueryresult.py` & `facebook_business-9.0.3/facebook_business/adobjects/adnetworkanalyticssyncqueryresult.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adoptablepet.py` & `facebook_business-9.0.3/facebook_business/adobjects/adoptablepet.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adplacement.py` & `facebook_business-9.0.3/facebook_business/adobjects/adplacement.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adplacepageset.py` & `facebook_business-9.0.3/facebook_business/adobjects/adplacepageset.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adplacepagesetmetadata.py` & `facebook_business-9.0.3/facebook_business/adobjects/adplacepagesetmetadata.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adpreview.py` & `facebook_business-9.0.3/facebook_business/adobjects/adpreview.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,18 +47,21 @@
         audience_network_instream_video_mobile = 'AUDIENCE_NETWORK_INSTREAM_VIDEO_MOBILE'
         audience_network_outstream_video = 'AUDIENCE_NETWORK_OUTSTREAM_VIDEO'
         audience_network_rewarded_video = 'AUDIENCE_NETWORK_REWARDED_VIDEO'
         desktop_feed_standard = 'DESKTOP_FEED_STANDARD'
         facebook_story_mobile = 'FACEBOOK_STORY_MOBILE'
         instagram_explore_contextual = 'INSTAGRAM_EXPLORE_CONTEXTUAL'
         instagram_explore_immersive = 'INSTAGRAM_EXPLORE_IMMERSIVE'
+        instagram_reels = 'INSTAGRAM_REELS'
         instagram_standard = 'INSTAGRAM_STANDARD'
         instagram_story = 'INSTAGRAM_STORY'
         instant_article_recirculation_ad = 'INSTANT_ARTICLE_RECIRCULATION_AD'
         instant_article_standard = 'INSTANT_ARTICLE_STANDARD'
+        instream_banner_desktop = 'INSTREAM_BANNER_DESKTOP'
+        instream_banner_mobile = 'INSTREAM_BANNER_MOBILE'
         instream_video_desktop = 'INSTREAM_VIDEO_DESKTOP'
         instream_video_image = 'INSTREAM_VIDEO_IMAGE'
         instream_video_mobile = 'INSTREAM_VIDEO_MOBILE'
         job_browser_desktop = 'JOB_BROWSER_DESKTOP'
         job_browser_mobile = 'JOB_BROWSER_MOBILE'
         marketplace_mobile = 'MARKETPLACE_MOBILE'
         messenger_mobile_inbox_media = 'MESSENGER_MOBILE_INBOX_MEDIA'
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adpromotedobject.py` & `facebook_business-9.0.3/facebook_business/adobjects/adpromotedobject.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adrecommendation.py` & `facebook_business-9.0.3/facebook_business/adobjects/adrecommendation.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adrecommendationdata.py` & `facebook_business-9.0.3/facebook_business/adobjects/adrecommendationdata.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adreportrun.py` & `facebook_business-9.0.3/facebook_business/adobjects/adreportrun.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adreportspec.py` & `facebook_business-9.0.3/facebook_business/adobjects/adreportspec.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adrule.py` & `facebook_business-9.0.3/facebook_business/adobjects/adrule.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adruleevaluationspec.py` & `facebook_business-9.0.3/facebook_business/adobjects/adruleevaluationspec.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adruleexecutionoptions.py` & `facebook_business-9.0.3/facebook_business/adobjects/adruleexecutionoptions.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adruleexecutionspec.py` & `facebook_business-9.0.3/facebook_business/adobjects/adruleexecutionspec.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adrulefilters.py` & `facebook_business-9.0.3/facebook_business/adobjects/adrulefilters.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adrulehistory.py` & `facebook_business-9.0.3/facebook_business/adobjects/adrulehistory.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adrulehistoryresult.py` & `facebook_business-9.0.3/facebook_business/adobjects/adrulehistoryresult.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adrulehistoryresultaction.py` & `facebook_business-9.0.3/facebook_business/adobjects/adrulehistoryresultaction.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adruleschedule.py` & `facebook_business-9.0.3/facebook_business/adobjects/adruleschedule.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adruleschedulespec.py` & `facebook_business-9.0.3/facebook_business/adobjects/adruleschedulespec.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adruletrigger.py` & `facebook_business-9.0.3/facebook_business/adobjects/adruletrigger.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adsactionstats.py` & `facebook_business-9.0.3/facebook_business/adobjects/adsactionstats.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,18 +40,20 @@
     class Field(AbstractObject.Field):
         field_1d_click = '1d_click'
         field_1d_view = '1d_view'
         field_28d_click = '28d_click'
         field_28d_view = '28d_view'
         field_7d_click = '7d_click'
         field_7d_view = '7d_view'
+        action_brand = 'action_brand'
         action_canvas_component_id = 'action_canvas_component_id'
         action_canvas_component_name = 'action_canvas_component_name'
         action_carousel_card_id = 'action_carousel_card_id'
         action_carousel_card_name = 'action_carousel_card_name'
+        action_category = 'action_category'
         action_converted_product_id = 'action_converted_product_id'
         action_destination = 'action_destination'
         action_device = 'action_device'
         action_event_channel = 'action_event_channel'
         action_link_click_destination = 'action_link_click_destination'
         action_location_code = 'action_location_code'
         action_reaction = 'action_reaction'
@@ -69,18 +71,20 @@
     _field_types = {
         '1d_click': 'string',
         '1d_view': 'string',
         '28d_click': 'string',
         '28d_view': 'string',
         '7d_click': 'string',
         '7d_view': 'string',
+        'action_brand': 'string',
         'action_canvas_component_id': 'string',
         'action_canvas_component_name': 'string',
         'action_carousel_card_id': 'string',
         'action_carousel_card_name': 'string',
+        'action_category': 'string',
         'action_converted_product_id': 'string',
         'action_destination': 'string',
         'action_device': 'string',
         'action_event_channel': 'string',
         'action_link_click_destination': 'string',
         'action_location_code': 'string',
         'action_reaction': 'string',
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adset.py` & `facebook_business-9.0.3/facebook_business/adobjects/adset.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,18 +116,20 @@
         lowest_cost_with_bid_cap = 'LOWEST_COST_WITH_BID_CAP'
 
     class BillingEvent:
         app_installs = 'APP_INSTALLS'
         clicks = 'CLICKS'
         impressions = 'IMPRESSIONS'
         link_clicks = 'LINK_CLICKS'
+        listing_interaction = 'LISTING_INTERACTION'
         none = 'NONE'
         offer_claims = 'OFFER_CLAIMS'
         page_likes = 'PAGE_LIKES'
         post_engagement = 'POST_ENGAGEMENT'
+        purchase = 'PURCHASE'
         thruplay = 'THRUPLAY'
 
     class ConfiguredStatus:
         active = 'ACTIVE'
         archived = 'ARCHIVED'
         deleted = 'DELETED'
         paused = 'PAUSED'
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adsimagecrops.py` & `facebook_business-9.0.3/facebook_business/adobjects/adsimagecrops.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adsinsights.py` & `facebook_business-9.0.3/facebook_business/adobjects/adsinsights.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
         adset_budget_value = 'adset_budget_value'
         adset_delivery = 'adset_delivery'
         adset_end = 'adset_end'
         adset_id = 'adset_id'
         adset_name = 'adset_name'
         adset_start = 'adset_start'
         age_targeting = 'age_targeting'
+        attribution_setting = 'attribution_setting'
         auction_bid = 'auction_bid'
         auction_competitiveness = 'auction_competitiveness'
         auction_max_competitor_bid = 'auction_max_competitor_bid'
         buying_type = 'buying_type'
         campaign_id = 'campaign_id'
         campaign_name = 'campaign_name'
         canvas_avg_view_percent = 'canvas_avg_view_percent'
@@ -289,14 +290,15 @@
         'adset_budget_value': 'string',
         'adset_delivery': 'string',
         'adset_end': 'string',
         'adset_id': 'string',
         'adset_name': 'string',
         'adset_start': 'string',
         'age_targeting': 'string',
+        'attribution_setting': 'string',
         'auction_bid': 'string',
         'auction_competitiveness': 'string',
         'auction_max_competitor_bid': 'string',
         'buying_type': 'string',
         'campaign_id': 'string',
         'campaign_name': 'string',
         'canvas_avg_view_percent': 'string',
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adsoptimaldeliverygrowthopportunity.py` & `facebook_business-9.0.3/facebook_business/adobjects/adsoptimaldeliverygrowthopportunity.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adspixel.py` & `facebook_business-9.0.3/facebook_business/adobjects/adspixel.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,14 +300,44 @@
             return request
         elif pending:
             return request
         else:
             self.assure_call()
             return request.execute()
 
+    def create_shadow_traffic_helper(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
+        from facebook_business.utils import api_utils
+        if batch is None and (success is not None or failure is not None):
+          api_utils.warning('`success` and `failure` callback only work for batch call.')
+        param_types = {
+        }
+        enums = {
+        }
+        request = FacebookRequest(
+            node_id=self['id'],
+            method='POST',
+            endpoint='/shadowtraffichelper',
+            api=self._api,
+            param_checker=TypeChecker(param_types, enums),
+            target_class=AbstractCrudObject,
+            api_type='EDGE',
+            response_parser=ObjectParser(target_class=AbstractCrudObject, api=self._api),
+        )
+        request.add_params(params)
+        request.add_fields(fields)
+
+        if batch is not None:
+            request.add_to_batch(batch, success=success, failure=failure)
+            return request
+        elif pending:
+            return request
+        else:
+            self.assure_call()
+            return request.execute()
+
     def delete_shared_accounts(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
         from facebook_business.utils import api_utils
         if batch is None and (success is not None or failure is not None):
           api_utils.warning('`success` and `failure` callback only work for batch call.')
         param_types = {
             'account_id': 'string',
             'business': 'string',
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adspixelstats.py` & `facebook_business-9.0.3/facebook_business/adobjects/adspixelstats.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adspixelstatsresult.py` & `facebook_business-9.0.3/facebook_business/adobjects/adspixelstatsresult.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adstudy.py` & `facebook_business-9.0.3/facebook_business/adobjects/adstudy.py`

 * *Files 6% similar despite different names*

```diff
@@ -240,55 +240,14 @@
             return request
         elif pending:
             return request
         else:
             self.assure_call()
             return request.execute()
 
-    def create_objective(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
-        from facebook_business.utils import api_utils
-        if batch is None and (success is not None or failure is not None):
-          api_utils.warning('`success` and `failure` callback only work for batch call.')
-        from facebook_business.adobjects.adstudyobjective import AdStudyObjective
-        param_types = {
-            'adspixels': 'list<Object>',
-            'applications': 'list<Object>',
-            'customconversions': 'list<Object>',
-            'is_primary': 'bool',
-            'name': 'string',
-            'offline_conversion_data_sets': 'list<Object>',
-            'product_catalogs': 'list<Object>',
-            'product_sets': 'list<Object>',
-            'type': 'type_enum',
-        }
-        enums = {
-            'type_enum': AdStudyObjective.Type.__dict__.values(),
-        }
-        request = FacebookRequest(
-            node_id=self['id'],
-            method='POST',
-            endpoint='/objectives',
-            api=self._api,
-            param_checker=TypeChecker(param_types, enums),
-            target_class=AdStudyObjective,
-            api_type='EDGE',
-            response_parser=ObjectParser(target_class=AdStudyObjective, api=self._api),
-        )
-        request.add_params(params)
-        request.add_fields(fields)
-
-        if batch is not None:
-            request.add_to_batch(batch, success=success, failure=failure)
-            return request
-        elif pending:
-            return request
-        else:
-            self.assure_call()
-            return request.execute()
-
     _field_types = {
         'business': 'Business',
         'canceled_time': 'datetime',
         'cooldown_start_time': 'datetime',
         'created_by': 'User',
         'created_time': 'datetime',
         'description': 'string',
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adstudycell.py` & `facebook_business-9.0.3/facebook_business/adobjects/adstudycell.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adstudyobjective.py` & `facebook_business-9.0.3/facebook_business/adobjects/adstudyobjective.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,44 +55,14 @@
         mae = 'MAE'
         mai = 'MAI'
         nonsales = 'NONSALES'
         partner = 'PARTNER'
         sales = 'SALES'
         telco = 'TELCO'
 
-    def api_delete(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
-        from facebook_business.utils import api_utils
-        if batch is None and (success is not None or failure is not None):
-          api_utils.warning('`success` and `failure` callback only work for batch call.')
-        param_types = {
-        }
-        enums = {
-        }
-        request = FacebookRequest(
-            node_id=self['id'],
-            method='DELETE',
-            endpoint='/',
-            api=self._api,
-            param_checker=TypeChecker(param_types, enums),
-            target_class=AbstractCrudObject,
-            api_type='NODE',
-            response_parser=ObjectParser(reuse_object=self),
-        )
-        request.add_params(params)
-        request.add_fields(fields)
-
-        if batch is not None:
-            request.add_to_batch(batch, success=success, failure=failure)
-            return request
-        elif pending:
-            return request
-        else:
-            self.assure_call()
-            return request.execute()
-
     def api_get(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
         from facebook_business.utils import api_utils
         if batch is None and (success is not None or failure is not None):
           api_utils.warning('`success` and `failure` callback only work for batch call.')
         param_types = {
             'breakdowns': 'list<breakdowns_enum>',
             'ds': 'string',
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/adstudyobjectiveid.py` & `facebook_business-9.0.3/facebook_business/adobjects/adstudyobjectiveid.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/advideo.py` & `facebook_business-9.0.3/facebook_business/adobjects/advideo.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,14 @@
         title = 'title'
         universal_video_id = 'universal_video_id'
         updated_time = 'updated_time'
         adaptive_type = 'adaptive_type'
         animated_effect_id = 'animated_effect_id'
         application_id = 'application_id'
         asked_fun_fact_prompt_id = 'asked_fun_fact_prompt_id'
-        attribution_app_id = 'attribution_app_id'
         audio_story_wave_animation_handle = 'audio_story_wave_animation_handle'
         chunk_session_id = 'chunk_session_id'
         composer_entry_picker = 'composer_entry_picker'
         composer_entry_point = 'composer_entry_point'
         composer_entry_time = 'composer_entry_time'
         composer_session_events_log = 'composer_session_events_log'
         composer_session_id = 'composer_session_id'
@@ -149,14 +148,15 @@
         video_id_original = 'video_id_original'
         video_start_time_ms = 'video_start_time_ms'
         waterfall_id = 'waterfall_id'
         filename = 'filename'
         filepath = 'filepath'
 
     class ContainerType:
+        aco_autoextracted_video = 'ACO_AUTOEXTRACTED_VIDEO'
         aco_video_variation = 'ACO_VIDEO_VARIATION'
         ad_break_preview = 'AD_BREAK_PREVIEW'
         ad_derivative = 'AD_DERIVATIVE'
         age_up = 'AGE_UP'
         album_multimedia_post = 'ALBUM_MULTIMEDIA_POST'
         aloha_call_video = 'ALOHA_CALL_VIDEO'
         aloha_superframe = 'ALOHA_SUPERFRAME'
@@ -186,14 +186,15 @@
         dynamic_item_display_bundle = 'DYNAMIC_ITEM_DISPLAY_BUNDLE'
         dynamic_item_video = 'DYNAMIC_ITEM_VIDEO'
         dynamic_template_video = 'DYNAMIC_TEMPLATE_VIDEO'
         event_cover_video = 'EVENT_COVER_VIDEO'
         event_tour = 'EVENT_TOUR'
         facecast_dvr = 'FACECAST_DVR'
         fb_shorts = 'FB_SHORTS'
+        fb_shorts_group_post = 'FB_SHORTS_GROUP_POST'
         fb_shorts_post = 'FB_SHORTS_POST'
         fundraiser_cover_video = 'FUNDRAISER_COVER_VIDEO'
         game_clip = 'GAME_CLIP'
         gaming_update_video = 'GAMING_UPDATE_VIDEO'
         gemstone = 'GEMSTONE'
         goodwill_anniversary_deprecated = 'GOODWILL_ANNIVERSARY_DEPRECATED'
         goodwill_anniversary_promotion_deprecated = 'GOODWILL_ANNIVERSARY_PROMOTION_DEPRECATED'
@@ -1034,15 +1035,14 @@
         'title': 'string',
         'universal_video_id': 'string',
         'updated_time': 'datetime',
         'adaptive_type': 'string',
         'animated_effect_id': 'unsigned int',
         'application_id': 'string',
         'asked_fun_fact_prompt_id': 'unsigned int',
-        'attribution_app_id': 'string',
         'audio_story_wave_animation_handle': 'string',
         'chunk_session_id': 'string',
         'composer_entry_picker': 'string',
         'composer_entry_point': 'string',
         'composer_entry_time': 'unsigned int',
         'composer_session_events_log': 'string',
         'composer_session_id': 'string',
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/agencyclientdeclaration.py` & `facebook_business-9.0.3/facebook_business/adobjects/agencyclientdeclaration.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/agerange.py` & `facebook_business-9.0.3/facebook_business/adobjects/agerange.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/album.py` & `facebook_business-9.0.3/facebook_business/adobjects/album.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/androidapplink.py` & `facebook_business-9.0.3/facebook_business/adobjects/androidapplink.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/application.py` & `facebook_business-9.0.3/facebook_business/adobjects/application.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/apprequest.py` & `facebook_business-9.0.3/facebook_business/adobjects/apprequest.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/apprequestformerrecipient.py` & `facebook_business-9.0.3/facebook_business/adobjects/apprequestformerrecipient.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/assigneduser.py` & `facebook_business-9.0.3/facebook_business/adobjects/assigneduser.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/asyncrequest.py` & `facebook_business-9.0.3/facebook_business/adobjects/asyncrequest.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/asyncsession.py` & `facebook_business-9.0.3/facebook_business/adobjects/asyncsession.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/atlascampaign.py` & `facebook_business-9.0.3/facebook_business/adobjects/atlascampaign.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/attributionspec.py` & `facebook_business-9.0.3/facebook_business/adobjects/attributionspec.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/audienceinsightsstudyspec.py` & `facebook_business-9.0.3/facebook_business/adobjects/audienceinsightsstudyspec.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/audiencepermissionforactions.py` & `facebook_business-9.0.3/facebook_business/adobjects/audiencepermissionforactions.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/audiocopyright.py` & `facebook_business-9.0.3/facebook_business/adobjects/audiocopyright.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/automotivemodel.py` & `facebook_business-9.0.3/facebook_business/adobjects/automotivemodel.py`

 * *Files 13% similar despite different names*

```diff
@@ -65,14 +65,48 @@
         sanitized_images = 'sanitized_images'
         title = 'title'
         transmission = 'transmission'
         trim = 'trim'
         url = 'url'
         year = 'year'
 
+    class BodyStyle:
+        convertible = 'CONVERTIBLE'
+        coupe = 'COUPE'
+        crossover = 'CROSSOVER'
+        estate = 'ESTATE'
+        grandtourer = 'GRANDTOURER'
+        hatchback = 'HATCHBACK'
+        minibus = 'MINIBUS'
+        minivan = 'MINIVAN'
+        mpv = 'MPV'
+        none = 'NONE'
+        other = 'OTHER'
+        pickup = 'PICKUP'
+        roadster = 'ROADSTER'
+        saloon = 'SALOON'
+        sedan = 'SEDAN'
+        sportscar = 'SPORTSCAR'
+        supercar = 'SUPERCAR'
+        supermini = 'SUPERMINI'
+        suv = 'SUV'
+        truck = 'TRUCK'
+        van = 'VAN'
+        wagon = 'WAGON'
+
+    # @deprecated get_endpoint function is deprecated
+    @classmethod
+    def get_endpoint(cls):
+        return 'automotive_models'
+
+    # @deprecated api_create is being deprecated
+    def api_create(self, parent_id, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
+        from facebook_business.adobjects.productcatalog import ProductCatalog
+        return ProductCatalog(api=self._api, fbid=parent_id).create_automotive_model(fields, params, batch, success, failure, pending)
+
     def api_get(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
         from facebook_business.utils import api_utils
         if batch is None and (success is not None or failure is not None):
           api_utils.warning('`success` and `failure` callback only work for batch call.')
         param_types = {
         }
         enums = {
@@ -127,10 +161,11 @@
         'trim': 'string',
         'url': 'string',
         'year': 'unsigned int',
     }
     @classmethod
     def _get_field_enum_info(cls):
         field_enum_info = {}
+        field_enum_info['BodyStyle'] = AutomotiveModel.BodyStyle.__dict__.values()
         return field_enum_info
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/billedamountdetails.py` & `facebook_business-9.0.3/facebook_business/adobjects/billedamountdetails.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/brandsafetyblocklistusage.py` & `facebook_business-9.0.3/facebook_business/adobjects/brandsafetyblocklistusage.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/broadtargetingcategories.py` & `facebook_business-9.0.3/facebook_business/adobjects/broadtargetingcategories.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/business.py` & `facebook_business-9.0.3/facebook_business/adobjects/business.py`

 * *Files 0% similar despite different names*

```diff
@@ -882,14 +882,48 @@
             return request
         elif pending:
             return request
         else:
             self.assure_call()
             return request.execute()
 
+    def create_business_user(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
+        from facebook_business.utils import api_utils
+        if batch is None and (success is not None or failure is not None):
+          api_utils.warning('`success` and `failure` callback only work for batch call.')
+        from facebook_business.adobjects.businessuser import BusinessUser
+        param_types = {
+            'email': 'string',
+            'role': 'role_enum',
+        }
+        enums = {
+            'role_enum': BusinessUser.Role.__dict__.values(),
+        }
+        request = FacebookRequest(
+            node_id=self['id'],
+            method='POST',
+            endpoint='/business_users',
+            api=self._api,
+            param_checker=TypeChecker(param_types, enums),
+            target_class=BusinessUser,
+            api_type='EDGE',
+            response_parser=ObjectParser(target_class=BusinessUser, api=self._api),
+        )
+        request.add_params(params)
+        request.add_fields(fields)
+
+        if batch is not None:
+            request.add_to_batch(batch, success=success, failure=failure)
+            return request
+        elif pending:
+            return request
+        else:
+            self.assure_call()
+            return request.execute()
+
     def create_claim_custom_conversion(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
         from facebook_business.utils import api_utils
         if batch is None and (success is not None or failure is not None):
           api_utils.warning('`success` and `failure` callback only work for batch call.')
         from facebook_business.adobjects.customconversion import CustomConversion
         param_types = {
             'custom_conversion_id': 'string',
@@ -1599,14 +1633,57 @@
             return request
         elif pending:
             return request
         else:
             self.assure_call()
             return request.execute()
 
+    def create_franchise_program(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
+        from facebook_business.utils import api_utils
+        if batch is None and (success is not None or failure is not None):
+          api_utils.warning('`success` and `failure` callback only work for batch call.')
+        param_types = {
+            'business_asset_group': 'string',
+            'creative_folder': 'string',
+            'creative_spec_template_data': 'map',
+            'description': 'string',
+            'end_date': 'datetime',
+            'name': 'string',
+            'program_approval_type': 'program_approval_type_enum',
+            'shared_custom_audience': 'string',
+            'start_date': 'datetime',
+        }
+        enums = {
+            'program_approval_type_enum': [
+                'APPROVAL',
+                'PUBLIC',
+            ],
+        }
+        request = FacebookRequest(
+            node_id=self['id'],
+            method='POST',
+            endpoint='/franchise_programs',
+            api=self._api,
+            param_checker=TypeChecker(param_types, enums),
+            target_class=AbstractCrudObject,
+            api_type='EDGE',
+            response_parser=ObjectParser(target_class=AbstractCrudObject, api=self._api),
+        )
+        request.add_params(params)
+        request.add_fields(fields)
+
+        if batch is not None:
+            request.add_to_batch(batch, success=success, failure=failure)
+            return request
+        elif pending:
+            return request
+        else:
+            self.assure_call()
+            return request.execute()
+
     def get_initiated_audience_sharing_requests(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
         from facebook_business.utils import api_utils
         if batch is None and (success is not None or failure is not None):
           api_utils.warning('`success` and `failure` callback only work for batch call.')
         from facebook_business.adobjects.businessassetsharingagreement import BusinessAssetSharingAgreement
         param_types = {
             'recipient_id': 'string',
@@ -2762,14 +2839,49 @@
             endpoint='/system_users',
             api=self._api,
             param_checker=TypeChecker(param_types, enums),
             target_class=SystemUser,
             api_type='EDGE',
             response_parser=ObjectParser(target_class=SystemUser, api=self._api),
         )
+        request.add_params(params)
+        request.add_fields(fields)
+
+        if batch is not None:
+            request.add_to_batch(batch, success=success, failure=failure)
+            return request
+        elif pending:
+            return request
+        else:
+            self.assure_call()
+            return request.execute()
+
+    def create_system_user(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
+        from facebook_business.utils import api_utils
+        if batch is None and (success is not None or failure is not None):
+          api_utils.warning('`success` and `failure` callback only work for batch call.')
+        from facebook_business.adobjects.systemuser import SystemUser
+        param_types = {
+            'name': 'string',
+            'role': 'role_enum',
+            'system_user_id': 'int',
+        }
+        enums = {
+            'role_enum': SystemUser.Role.__dict__.values(),
+        }
+        request = FacebookRequest(
+            node_id=self['id'],
+            method='POST',
+            endpoint='/system_users',
+            api=self._api,
+            param_checker=TypeChecker(param_types, enums),
+            target_class=SystemUser,
+            api_type='EDGE',
+            response_parser=ObjectParser(target_class=SystemUser, api=self._api),
+        )
         request.add_params(params)
         request.add_fields(fields)
 
         if batch is not None:
             request.add_to_batch(batch, success=success, failure=failure)
             return request
         elif pending:
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/businessadaccountrequest.py` & `facebook_business-9.0.3/facebook_business/adobjects/businessadaccountrequest.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/businessagreement.py` & `facebook_business-9.0.3/facebook_business/adobjects/businessagreement.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/businessapplicationrequest.py` & `facebook_business-9.0.3/facebook_business/adobjects/businessapplicationrequest.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/businessassetgroup.py` & `facebook_business-9.0.3/facebook_business/adobjects/businessassetgroup.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/businessassetsharingagreement.py` & `facebook_business-9.0.3/facebook_business/adobjects/businessassetsharingagreement.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/businessownedobjectonbehalfofrequest.py` & `facebook_business-9.0.3/facebook_business/adobjects/businessownedobjectonbehalfofrequest.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/businesspagerequest.py` & `facebook_business-9.0.3/facebook_business/adobjects/businesspagerequest.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/businessrolerequest.py` & `facebook_business-9.0.3/facebook_business/adobjects/businessrolerequest.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/businessunit.py` & `facebook_business-9.0.3/facebook_business/adobjects/businessunit.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/businessuser.py` & `facebook_business-9.0.3/facebook_business/adobjects/businessuser.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,24 @@
         manage = 'MANAGE'
         partner_center_admin = 'PARTNER_CENTER_ADMIN'
         partner_center_analyst = 'PARTNER_CENTER_ANALYST'
         partner_center_education = 'PARTNER_CENTER_EDUCATION'
         partner_center_marketing = 'PARTNER_CENTER_MARKETING'
         partner_center_operations = 'PARTNER_CENTER_OPERATIONS'
 
+    # @deprecated get_endpoint function is deprecated
+    @classmethod
+    def get_endpoint(cls):
+        return 'business_users'
+
+    # @deprecated api_create is being deprecated
+    def api_create(self, parent_id, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
+        from facebook_business.adobjects.business import Business
+        return Business(api=self._api, fbid=parent_id).create_business_user(fields, params, batch, success, failure, pending)
+
     def api_delete(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
         from facebook_business.utils import api_utils
         if batch is None and (success is not None or failure is not None):
           api_utils.warning('`success` and `failure` callback only work for batch call.')
         param_types = {
         }
         enums = {
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/campaign.py` & `facebook_business-9.0.3/facebook_business/adobjects/campaign.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,14 @@
         conversions = 'CONVERSIONS'
         event_responses = 'EVENT_RESPONSES'
         lead_generation = 'LEAD_GENERATION'
         link_clicks = 'LINK_CLICKS'
         local_awareness = 'LOCAL_AWARENESS'
         messages = 'MESSAGES'
         offer_claims = 'OFFER_CLAIMS'
-        outcome_leads = 'OUTCOME_LEADS'
         page_likes = 'PAGE_LIKES'
         post_engagement = 'POST_ENGAGEMENT'
         product_catalog_sales = 'PRODUCT_CATALOG_SALES'
         reach = 'REACH'
         store_visits = 'STORE_VISITS'
         video_views = 'VIDEO_VIEWS'
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/campaigngroupbrandconfiguration.py` & `facebook_business-9.0.3/facebook_business/adobjects/campaigngroupbrandconfiguration.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/campaigngroupcollaborativeadspartnerinfo.py` & `facebook_business-9.0.3/facebook_business/adobjects/campaigngroupcollaborativeadspartnerinfo.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/canvas.py` & `facebook_business-9.0.3/facebook_business/adobjects/canvas.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/canvasadsettings.py` & `facebook_business-9.0.3/facebook_business/adobjects/canvasadsettings.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/canvasbodyelement.py` & `facebook_business-9.0.3/facebook_business/adobjects/canvasbodyelement.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/canvascollectionthumbnail.py` & `facebook_business-9.0.3/facebook_business/adobjects/canvascollectionthumbnail.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/catalogbasedtargeting.py` & `facebook_business-9.0.3/facebook_business/adobjects/catalogbasedtargeting.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/catalogitemappealstatus.py` & `facebook_business-9.0.3/facebook_business/adobjects/catalogitemappealstatus.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/catalogitemapplinks.py` & `facebook_business-9.0.3/facebook_business/adobjects/catalogitemapplinks.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/catalogitemchannelstointegritystatus.py` & `facebook_business-9.0.3/facebook_business/adobjects/catalogitemchannelstointegritystatus.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/catalogsubverticallist.py` & `facebook_business-9.0.3/facebook_business/adobjects/catalogsubverticallist.py`

 * *Files 11% similar despite different names*

```diff
@@ -51,23 +51,26 @@
         clothing = 'clothing'
         clothing_accessories = 'clothing_accessories'
         clothing_group = 'clothing_group'
         computer_components = 'computer_components'
         computers_and_tablets = 'computers_and_tablets'
         computers_laptops_and_tablets = 'computers_laptops_and_tablets'
         diapering_and_potty_training = 'diapering_and_potty_training'
+        digital_product_offer = 'digital_product_offer'
         electronic_accessories_and_cables = 'electronic_accessories_and_cables'
         electronics_accessories = 'electronics_accessories'
         furniture = 'furniture'
         health = 'health'
         home = 'home'
         home_goods = 'home_goods'
         household_and_cleaning_supplies = 'household_and_cleaning_supplies'
         jewelry = 'jewelry'
         large_appliances = 'large_appliances'
+        local_service_business_item = 'local_service_business_item'
+        local_service_business_restaurant = 'local_service_business_restaurant'
         loyalty_offer = 'loyalty_offer'
         meetup_space = 'meetup_space'
         nursery = 'nursery'
         printers_and_scanners = 'printers_and_scanners'
         printers_scanners_and_fax_machines = 'printers_scanners_and_fax_machines'
         product_discount = 'product_discount'
         projectors = 'projectors'
@@ -105,23 +108,26 @@
         'clothing': 'Object',
         'clothing_accessories': 'Object',
         'clothing_group': 'Object',
         'computer_components': 'Object',
         'computers_and_tablets': 'Object',
         'computers_laptops_and_tablets': 'Object',
         'diapering_and_potty_training': 'Object',
+        'digital_product_offer': 'Object',
         'electronic_accessories_and_cables': 'Object',
         'electronics_accessories': 'Object',
         'furniture': 'Object',
         'health': 'Object',
         'home': 'Object',
         'home_goods': 'Object',
         'household_and_cleaning_supplies': 'Object',
         'jewelry': 'Object',
         'large_appliances': 'Object',
+        'local_service_business_item': 'Object',
+        'local_service_business_restaurant': 'Object',
         'loyalty_offer': 'Object',
         'meetup_space': 'Object',
         'nursery': 'Object',
         'printers_and_scanners': 'Object',
         'printers_scanners_and_fax_machines': 'Object',
         'product_discount': 'Object',
         'projectors': 'Object',
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/checkbatchrequeststatus.py` & `facebook_business-9.0.3/facebook_business/adobjects/checkbatchrequeststatus.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/childevent.py` & `facebook_business-9.0.3/facebook_business/adobjects/childevent.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/clicktrackingtag.py` & `facebook_business-9.0.3/facebook_business/adobjects/clicktrackingtag.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/collaborativeadspartnerinfolistitem.py` & `facebook_business-9.0.3/facebook_business/adobjects/collaborativeadspartnerinfolistitem.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/collaborativeadssharesettings.py` & `facebook_business-9.0.3/facebook_business/adobjects/collaborativeadssharesettings.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/comment.py` & `facebook_business-9.0.3/facebook_business/adobjects/comment.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 
     class CommentPrivacyValue:
         default_privacy = 'DEFAULT_PRIVACY'
         friends_and_post_owner = 'FRIENDS_AND_POST_OWNER'
         friends_only = 'FRIENDS_ONLY'
         graphql_multiple_value_hack_do_not_use = 'GRAPHQL_MULTIPLE_VALUE_HACK_DO_NOT_USE'
         owner_or_commenter = 'OWNER_OR_COMMENTER'
+        pending_approval = 'PENDING_APPROVAL'
         side_conversation = 'SIDE_CONVERSATION'
         side_conversation_and_post_owner = 'SIDE_CONVERSATION_AND_POST_OWNER'
 
     class Filter:
         stream = 'stream'
         toplevel = 'toplevel'
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/commercemerchantsettings.py` & `facebook_business-9.0.3/facebook_business/adobjects/commercemerchantsettings.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         contact_email = 'contact_email'
         cta = 'cta'
         disable_checkout_urls = 'disable_checkout_urls'
         display_name = 'display_name'
         external_merchant_id = 'external_merchant_id'
         facebook_channel = 'facebook_channel'
         has_discount_code = 'has_discount_code'
+        has_onsite_intent = 'has_onsite_intent'
         id = 'id'
         instagram_channel = 'instagram_channel'
         merchant_alert_email = 'merchant_alert_email'
         merchant_page = 'merchant_page'
         merchant_status = 'merchant_status'
         onsite_commerce_merchant = 'onsite_commerce_merchant'
         payment_provider = 'payment_provider'
@@ -398,14 +399,15 @@
         'contact_email': 'string',
         'cta': 'string',
         'disable_checkout_urls': 'bool',
         'display_name': 'string',
         'external_merchant_id': 'string',
         'facebook_channel': 'Object',
         'has_discount_code': 'bool',
+        'has_onsite_intent': 'bool',
         'id': 'string',
         'instagram_channel': 'Object',
         'merchant_alert_email': 'string',
         'merchant_page': 'Profile',
         'merchant_status': 'string',
         'onsite_commerce_merchant': 'Object',
         'payment_provider': 'string',
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/commercemerchantsettingssetupstatus.py` & `facebook_business-9.0.3/facebook_business/adobjects/commercemerchantsettingssetupstatus.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/commerceorder.py` & `facebook_business-9.0.3/facebook_business/adobjects/commerceorder.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/commerceordertransactiondetail.py` & `facebook_business-9.0.3/facebook_business/adobjects/commerceordertransactiondetail.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/commercepayout.py` & `facebook_business-9.0.3/facebook_business/adobjects/commercepayout.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/commercesettings.py` & `facebook_business-9.0.3/facebook_business/adobjects/commercesettings.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/connectionstargeting.py` & `facebook_business-9.0.3/facebook_business/adobjects/connectionstargeting.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/contentdeliveryreport.py` & `facebook_business-9.0.3/facebook_business/adobjects/contentdeliveryreport.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/conversionactionquery.py` & `facebook_business-9.0.3/facebook_business/adobjects/conversionactionquery.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/copyrightreferencecontainer.py` & `facebook_business-9.0.3/facebook_business/adobjects/copyrightreferencecontainer.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/coverphoto.py` & `facebook_business-9.0.3/facebook_business/adobjects/coverphoto.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/cpasadvertiserpartnershiprecommendation.py` & `facebook_business-9.0.3/facebook_business/adobjects/cpasadvertiserpartnershiprecommendation.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/cpascollaborationrequest.py` & `facebook_business-9.0.3/facebook_business/adobjects/cpascollaborationrequest.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/cpasparentcatalogsettings.py` & `facebook_business-9.0.3/facebook_business/adobjects/cpasparentcatalogsettings.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/creativehistory.py` & `facebook_business-9.0.3/facebook_business/adobjects/creativehistory.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/creditpartitionactionoptions.py` & `facebook_business-9.0.3/facebook_business/adobjects/creditpartitionactionoptions.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/currency.py` & `facebook_business-9.0.3/facebook_business/adobjects/currency.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/currencyamount.py` & `facebook_business-9.0.3/facebook_business/adobjects/currencyamount.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/customaudience.py` & `facebook_business-9.0.3/facebook_business/adobjects/customaudience.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/customaudienceadaccount.py` & `facebook_business-9.0.3/facebook_business/adobjects/customaudienceadaccount.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/customaudiencedatasource.py` & `facebook_business-9.0.3/facebook_business/adobjects/customaudiencedatasource.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/customaudiencesession.py` & `facebook_business-9.0.3/facebook_business/adobjects/customaudiencesession.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/customaudiencesharedaccountinfo.py` & `facebook_business-9.0.3/facebook_business/adobjects/customaudiencesharedaccountinfo.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/customaudiencesharingstatus.py` & `facebook_business-9.0.3/facebook_business/adobjects/customaudiencesharingstatus.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/customaudiencestatus.py` & `facebook_business-9.0.3/facebook_business/adobjects/customaudiencestatus.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/customaudiencestos.py` & `facebook_business-9.0.3/facebook_business/adobjects/customaudiencestos.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/customconversion.py` & `facebook_business-9.0.3/facebook_business/adobjects/customconversion.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/customconversionstatsresult.py` & `facebook_business-9.0.3/facebook_business/adobjects/customconversionstatsresult.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/customusersettings.py` & `facebook_business-9.0.3/facebook_business/adobjects/customusersettings.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/dacheck.py` & `facebook_business-9.0.3/facebook_business/adobjects/dacheck.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/daypart.py` & `facebook_business-9.0.3/facebook_business/adobjects/daypart.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/deliverycheck.py` & `facebook_business-9.0.3/facebook_business/adobjects/deliverycheck.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/deliverycheckextrainfo.py` & `facebook_business-9.0.3/facebook_business/adobjects/deliverycheckextrainfo.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/destination.py` & `facebook_business-9.0.3/facebook_business/adobjects/destination.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/destinationcatalogsettings.py` & `facebook_business-9.0.3/facebook_business/adobjects/destinationcatalogsettings.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/domain.py` & `facebook_business-9.0.3/facebook_business/adobjects/domain.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/dynamiccontentset.py` & `facebook_business-9.0.3/facebook_business/adobjects/dynamiccontentset.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/dynamicpostchildattachment.py` & `facebook_business-9.0.3/facebook_business/adobjects/dynamicpostchildattachment.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/dynamicpriceconfigbydate.py` & `facebook_business-9.0.3/facebook_business/adobjects/dynamicpriceconfigbydate.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/engagement.py` & `facebook_business-9.0.3/facebook_business/adobjects/engagement.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/entityattextrange.py` & `facebook_business-9.0.3/facebook_business/adobjects/entityattextrange.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/event.py` & `facebook_business-9.0.3/facebook_business/adobjects/event.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/eventsourcegroup.py` & `facebook_business-9.0.3/facebook_business/adobjects/eventsourcegroup.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/experience.py` & `facebook_business-9.0.3/facebook_business/adobjects/experience.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/extendedcredit.py` & `facebook_business-9.0.3/facebook_business/adobjects/extendedcredit.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/extendedcreditallocationconfig.py` & `facebook_business-9.0.3/facebook_business/adobjects/extendedcreditallocationconfig.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/extendedcreditinvoicegroup.py` & `facebook_business-9.0.3/facebook_business/adobjects/extendedcreditinvoicegroup.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/externaleventsource.py` & `facebook_business-9.0.3/facebook_business/adobjects/externaleventsource.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/fameexportconfig.py` & `facebook_business-9.0.3/facebook_business/adobjects/fameexportconfig.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/flexibletargeting.py` & `facebook_business-9.0.3/facebook_business/adobjects/flexibletargeting.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/flight.py` & `facebook_business-9.0.3/facebook_business/adobjects/flight.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/fundingsourcedetails.py` & `facebook_business-9.0.3/facebook_business/adobjects/fundingsourcedetails.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/fundingsourcedetailscoupon.py` & `facebook_business-9.0.3/facebook_business/adobjects/fundingsourcedetailscoupon.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/group.py` & `facebook_business-9.0.3/facebook_business/adobjects/group.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,22 +178,14 @@
         work_recruiting = 'WORK_RECRUITING'
         work_resume_review = 'WORK_RESUME_REVIEW'
         work_social = 'WORK_SOCIAL'
         work_team = 'WORK_TEAM'
         work_teamwork = 'WORK_TEAMWORK'
         work_vc_call = 'WORK_VC_CALL'
 
-    class SuggestionCategory:
-        event = 'EVENT'
-        messenger = 'MESSENGER'
-        work = 'WORK'
-        workplace = 'WORKPLACE'
-        workplace_1_1 = 'WORKPLACE_1_1'
-        workplace_manager = 'WORKPLACE_MANAGER'
-
     def api_get(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
         from facebook_business.utils import api_utils
         if batch is None and (success is not None or failure is not None):
           api_utils.warning('`success` and `failure` callback only work for batch call.')
         param_types = {
             'icon_size': 'icon_size_enum',
         }
@@ -732,22 +724,19 @@
             'join_setting': 'join_setting_enum',
             'name': 'string',
             'parent_id': 'Object',
             'post_permissions': 'post_permissions_enum',
             'post_requires_admin_approval': 'bool',
             'privacy': 'string',
             'ref': 'string',
-            'suggestion_category': 'suggestion_category_enum',
-            'suggestion_identifier': 'string',
         }
         enums = {
             'group_type_enum': Group.GroupType.__dict__.values(),
             'join_setting_enum': Group.JoinSetting.__dict__.values(),
             'post_permissions_enum': Group.PostPermissions.__dict__.values(),
-            'suggestion_category_enum': Group.SuggestionCategory.__dict__.values(),
         }
         request = FacebookRequest(
             node_id=self['id'],
             method='POST',
             endpoint='/groups',
             api=self._api,
             param_checker=TypeChecker(param_types, enums),
@@ -1119,15 +1108,14 @@
           api_utils.warning('`success` and `failure` callback only work for batch call.')
         from facebook_business.adobjects.advideo import AdVideo
         param_types = {
             'adaptive_type': 'string',
             'animated_effect_id': 'unsigned int',
             'application_id': 'string',
             'asked_fun_fact_prompt_id': 'unsigned int',
-            'attribution_app_id': 'string',
             'audio_story_wave_animation_handle': 'string',
             'composer_entry_picker': 'string',
             'composer_entry_point': 'string',
             'composer_entry_time': 'unsigned int',
             'composer_session_events_log': 'string',
             'composer_session_id': 'string',
             'composer_source_surface': 'string',
@@ -1249,11 +1237,10 @@
     @classmethod
     def _get_field_enum_info(cls):
         field_enum_info = {}
         field_enum_info['JoinSetting'] = Group.JoinSetting.__dict__.values()
         field_enum_info['PostPermissions'] = Group.PostPermissions.__dict__.values()
         field_enum_info['Purpose'] = Group.Purpose.__dict__.values()
         field_enum_info['GroupType'] = Group.GroupType.__dict__.values()
-        field_enum_info['SuggestionCategory'] = Group.SuggestionCategory.__dict__.values()
         return field_enum_info
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/helpers/__init__.py` & `facebook_business-9.0.3/facebook_business/adobjects/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/helpers/adaccountmixin.py` & `facebook_business-9.0.3/facebook_business/adobjects/helpers/adaccountmixin.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/helpers/adaccountusermixin.py` & `facebook_business-9.0.3/facebook_business/adobjects/helpers/adaccountusermixin.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/helpers/adimagemixin.py` & `facebook_business-9.0.3/facebook_business/adobjects/helpers/adimagemixin.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/helpers/adpreviewmixin.py` & `facebook_business-9.0.3/facebook_business/adobjects/helpers/adpreviewmixin.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/helpers/adreportrunmixin.py` & `facebook_business-9.0.3/facebook_business/adobjects/helpers/adreportrunmixin.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/helpers/adsinsightsmixin.py` & `facebook_business-9.0.3/facebook_business/adobjects/helpers/adsinsightsmixin.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/helpers/businessmixin.py` & `facebook_business-9.0.3/facebook_business/adobjects/helpers/businessmixin.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/helpers/customaudiencemixin.py` & `facebook_business-9.0.3/facebook_business/adobjects/helpers/customaudiencemixin.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/helpers/productcatalogmixin.py` & `facebook_business-9.0.3/facebook_business/adobjects/helpers/productcatalogmixin.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/helpers/reachfrequencypredictionmixin.py` & `facebook_business-9.0.3/facebook_business/adobjects/helpers/reachfrequencypredictionmixin.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/homelisting.py` & `facebook_business-9.0.3/facebook_business/adobjects/homelisting.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/hotel.py` & `facebook_business-9.0.3/facebook_business/adobjects/hotel.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/hotelroom.py` & `facebook_business-9.0.3/facebook_business/adobjects/hotelroom.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/idname.py` & `facebook_business-9.0.3/facebook_business/adobjects/idname.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/igcomment.py` & `facebook_business-9.0.3/facebook_business/adobjects/igcomment.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/igmedia.py` & `facebook_business-9.0.3/facebook_business/adobjects/igmedia.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/iguser.py` & `facebook_business-9.0.3/facebook_business/adobjects/iguser.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,45 @@
             return request
         elif pending:
             return request
         else:
             self.assure_call()
             return request.execute()
 
+    def get_content_publishing_limit(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
+        from facebook_business.utils import api_utils
+        if batch is None and (success is not None or failure is not None):
+          api_utils.warning('`success` and `failure` callback only work for batch call.')
+        param_types = {
+            'since': 'datetime',
+        }
+        enums = {
+        }
+        request = FacebookRequest(
+            node_id=self['id'],
+            method='GET',
+            endpoint='/content_publishing_limit',
+            api=self._api,
+            param_checker=TypeChecker(param_types, enums),
+            target_class=AbstractCrudObject,
+            api_type='EDGE',
+            response_parser=ObjectParser(target_class=AbstractCrudObject, api=self._api),
+        )
+        request.add_params(params)
+        request.add_fields(fields)
+
+        if batch is not None:
+            request.add_to_batch(batch, success=success, failure=failure)
+            return request
+        elif pending:
+            return request
+        else:
+            self.assure_call()
+            return request.execute()
+
     def get_insights(self, fields=None, params=None, is_async=False, batch=None, success=None, failure=None, pending=False):
         from facebook_business.utils import api_utils
         if batch is None and (success is not None or failure is not None):
           api_utils.warning('`success` and `failure` callback only work for batch call.')
         from facebook_business.adobjects.instagraminsightsresult import InstagramInsightsResult
         if is_async:
           return self.get_insights_async(fields, params, batch, success, failure, pending)
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/insightsresult.py` & `facebook_business-9.0.3/facebook_business/adobjects/insightsresult.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/instagraminsightsresult.py` & `facebook_business-9.0.3/facebook_business/adobjects/instagraminsightsresult.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/instagraminsightsvalue.py` & `facebook_business-9.0.3/facebook_business/adobjects/instagraminsightsvalue.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/instagramuser.py` & `facebook_business-9.0.3/facebook_business/adobjects/instagramuser.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/instantarticle.py` & `facebook_business-9.0.3/facebook_business/adobjects/instantarticle.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/instantarticleinsightsqueryresult.py` & `facebook_business-9.0.3/facebook_business/adobjects/instantarticleinsightsqueryresult.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/invoicecampaign.py` & `facebook_business-9.0.3/facebook_business/adobjects/invoicecampaign.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/iosapplink.py` & `facebook_business-9.0.3/facebook_business/adobjects/iosapplink.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/keyvalue.py` & `facebook_business-9.0.3/facebook_business/adobjects/keyvalue.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/lead.py` & `facebook_business-9.0.3/facebook_business/adobjects/lead.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/leadgenappointmentbookinginfo.py` & `facebook_business-9.0.3/facebook_business/adobjects/leadgenappointmentbookinginfo.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/leadgenconditionalquestionsgroupchoices.py` & `facebook_business-9.0.3/facebook_business/adobjects/leadgenconditionalquestionsgroupchoices.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/leadgenconditionalquestionsgroupquestions.py` & `facebook_business-9.0.3/facebook_business/adobjects/leadgenconditionalquestionsgroupquestions.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/leadgendraftquestion.py` & `facebook_business-9.0.3/facebook_business/adobjects/leadgendraftquestion.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/leadgenform.py` & `facebook_business-9.0.3/facebook_business/adobjects/leadgenform.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/leadgenpostsubmissioncheckresult.py` & `facebook_business-9.0.3/facebook_business/adobjects/leadgenpostsubmissioncheckresult.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/leadgenquestion.py` & `facebook_business-9.0.3/facebook_business/adobjects/leadgenquestion.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/leadgenquestionoption.py` & `facebook_business-9.0.3/facebook_business/adobjects/leadgenquestionoption.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/lifeevent.py` & `facebook_business-9.0.3/facebook_business/adobjects/lifeevent.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/link.py` & `facebook_business-9.0.3/facebook_business/adobjects/link.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/liveencoder.py` & `facebook_business-9.0.3/facebook_business/adobjects/liveencoder.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/livevideo.py` & `facebook_business-9.0.3/facebook_business/adobjects/livevideo.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/livevideoadbreakconfig.py` & `facebook_business-9.0.3/facebook_business/adobjects/livevideoadbreakconfig.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/livevideoerror.py` & `facebook_business-9.0.3/facebook_business/adobjects/livevideoerror.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/livevideoinputstream.py` & `facebook_business-9.0.3/facebook_business/adobjects/livevideoinputstream.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/livevideotargeting.py` & `facebook_business-9.0.3/facebook_business/adobjects/livevideotargeting.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/location.py` & `facebook_business-9.0.3/facebook_business/adobjects/location.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/lookalikespec.py` & `facebook_business-9.0.3/facebook_business/adobjects/lookalikespec.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/mailingaddress.py` & `facebook_business-9.0.3/facebook_business/adobjects/mailingaddress.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/measurementuploadevent.py` & `facebook_business-9.0.3/facebook_business/adobjects/measurementuploadevent.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/mediafingerprint.py` & `facebook_business-9.0.3/facebook_business/adobjects/mediafingerprint.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/messagingfeaturereview.py` & `facebook_business-9.0.3/facebook_business/adobjects/messagingfeaturereview.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/messengerdestinationpagewelcomemessage.py` & `facebook_business-9.0.3/facebook_business/adobjects/messengerdestinationpagewelcomemessage.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/messengerprofile.py` & `facebook_business-9.0.3/facebook_business/adobjects/messengerprofile.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/minimumbudget.py` & `facebook_business-9.0.3/facebook_business/adobjects/minimumbudget.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/musicvideocopyright.py` & `facebook_business-9.0.3/facebook_business/adobjects/musicvideocopyright.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/nativeoffer.py` & `facebook_business-9.0.3/facebook_business/adobjects/nativeoffer.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/nativeofferdiscount.py` & `facebook_business-9.0.3/facebook_business/adobjects/nativeofferdiscount.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/nativeofferview.py` & `facebook_business-9.0.3/facebook_business/adobjects/nativeofferview.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/nullnode.py` & `facebook_business-9.0.3/facebook_business/adobjects/nullnode.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/objectparser.py` & `facebook_business-9.0.3/facebook_business/adobjects/objectparser.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/offlineconversiondataset.py` & `facebook_business-9.0.3/facebook_business/adobjects/offlineconversiondataset.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/offsitepixel.py` & `facebook_business-9.0.3/facebook_business/adobjects/offsitepixel.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/opengraphcontext.py` & `facebook_business-9.0.3/facebook_business/adobjects/opengraphcontext.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/oracletransaction.py` & `facebook_business-9.0.3/facebook_business/adobjects/oracletransaction.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/outcomepredictionpoint.py` & `facebook_business-9.0.3/facebook_business/adobjects/outcomepredictionpoint.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/page.py` & `facebook_business-9.0.3/facebook_business/adobjects/page.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,15 @@
         display_subtext = 'display_subtext'
         displayed_message_response_time = 'displayed_message_response_time'
         emails = 'emails'
         engagement = 'engagement'
         fan_count = 'fan_count'
         featured_video = 'featured_video'
         features = 'features'
+        followers_count = 'followers_count'
         food_styles = 'food_styles'
         founded = 'founded'
         general_info = 'general_info'
         general_manager = 'general_manager'
         genre = 'genre'
         global_brand_page_name = 'global_brand_page_name'
         global_brand_root_id = 'global_brand_root_id'
@@ -1224,14 +1225,45 @@
             return request
         elif pending:
             return request
         else:
             self.assure_call()
             return request.execute()
 
+    def get_commerce_eligibility(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
+        from facebook_business.utils import api_utils
+        if batch is None and (success is not None or failure is not None):
+          api_utils.warning('`success` and `failure` callback only work for batch call.')
+        from facebook_business.adobjects.pagecommerceeligibility import PageCommerceEligibility
+        param_types = {
+        }
+        enums = {
+        }
+        request = FacebookRequest(
+            node_id=self['id'],
+            method='GET',
+            endpoint='/commerce_eligibility',
+            api=self._api,
+            param_checker=TypeChecker(param_types, enums),
+            target_class=PageCommerceEligibility,
+            api_type='EDGE',
+            response_parser=ObjectParser(target_class=PageCommerceEligibility, api=self._api),
+        )
+        request.add_params(params)
+        request.add_fields(fields)
+
+        if batch is not None:
+            request.add_to_batch(batch, success=success, failure=failure)
+            return request
+        elif pending:
+            return request
+        else:
+            self.assure_call()
+            return request.execute()
+
     def get_commerce_merchant_settings(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
         from facebook_business.utils import api_utils
         if batch is None and (success is not None or failure is not None):
           api_utils.warning('`success` and `failure` callback only work for batch call.')
         from facebook_business.adobjects.commercemerchantsettings import CommerceMerchantSettings
         param_types = {
         }
@@ -1960,14 +1992,86 @@
             return request
         elif pending:
             return request
         else:
             self.assure_call()
             return request.execute()
 
+    def get_image_copyrights(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
+        from facebook_business.utils import api_utils
+        if batch is None and (success is not None or failure is not None):
+          api_utils.warning('`success` and `failure` callback only work for batch call.')
+        from facebook_business.adobjects.imagecopyright import ImageCopyright
+        param_types = {
+        }
+        enums = {
+        }
+        request = FacebookRequest(
+            node_id=self['id'],
+            method='GET',
+            endpoint='/image_copyrights',
+            api=self._api,
+            param_checker=TypeChecker(param_types, enums),
+            target_class=ImageCopyright,
+            api_type='EDGE',
+            response_parser=ObjectParser(target_class=ImageCopyright, api=self._api),
+        )
+        request.add_params(params)
+        request.add_fields(fields)
+
+        if batch is not None:
+            request.add_to_batch(batch, success=success, failure=failure)
+            return request
+        elif pending:
+            return request
+        else:
+            self.assure_call()
+            return request.execute()
+
+    def create_image_copyright(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
+        from facebook_business.utils import api_utils
+        if batch is None and (success is not None or failure is not None):
+          api_utils.warning('`success` and `failure` callback only work for batch call.')
+        from facebook_business.adobjects.imagecopyright import ImageCopyright
+        param_types = {
+            'artist': 'string',
+            'creator': 'string',
+            'custom_id': 'string',
+            'description': 'string',
+            'filename': 'string',
+            'geo_ownership': 'list<geo_ownership_enum>',
+            'original_content_creation_date': 'unsigned int',
+            'reference_photo': 'string',
+            'title': 'string',
+        }
+        enums = {
+            'geo_ownership_enum': ImageCopyright.GeoOwnership.__dict__.values(),
+        }
+        request = FacebookRequest(
+            node_id=self['id'],
+            method='POST',
+            endpoint='/image_copyrights',
+            api=self._api,
+            param_checker=TypeChecker(param_types, enums),
+            target_class=ImageCopyright,
+            api_type='EDGE',
+            response_parser=ObjectParser(target_class=ImageCopyright, api=self._api),
+        )
+        request.add_params(params)
+        request.add_fields(fields)
+
+        if batch is not None:
+            request.add_to_batch(batch, success=success, failure=failure)
+            return request
+        elif pending:
+            return request
+        else:
+            self.assure_call()
+            return request.execute()
+
     def get_indexed_videos(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
         from facebook_business.utils import api_utils
         if batch is None and (success is not None or failure is not None):
           api_utils.warning('`success` and `failure` callback only work for batch call.')
         from facebook_business.adobjects.advideo import AdVideo
         param_types = {
         }
@@ -2549,14 +2653,15 @@
             'delivery_and_pickup_option_info': 'list<string>',
             'differently_open_offerings': 'map',
             'hours': 'map',
             'ignore_warnings': 'bool',
             'location': 'Object',
             'location_page_id': 'string',
             'old_store_number': 'unsigned int',
+            'page_username': 'string',
             'permanently_closed': 'bool',
             'phone': 'string',
             'pickup_options': 'list<pickup_options_enum>',
             'place_topics': 'list<string>',
             'price_range': 'string',
             'store_code': 'string',
             'store_location_descriptor': 'string',
@@ -4389,15 +4494,14 @@
         from facebook_business.adobjects.advideo import AdVideo
         param_types = {
             'ad_breaks': 'list',
             'adaptive_type': 'string',
             'animated_effect_id': 'unsigned int',
             'application_id': 'string',
             'asked_fun_fact_prompt_id': 'unsigned int',
-            'attribution_app_id': 'string',
             'audio_story_wave_animation_handle': 'string',
             'backdated_post': 'list',
             'call_to_action': 'Object',
             'composer_entry_picker': 'string',
             'composer_entry_point': 'string',
             'composer_entry_time': 'unsigned int',
             'composer_session_events_log': 'string',
@@ -4587,14 +4691,15 @@
         'display_subtext': 'string',
         'displayed_message_response_time': 'string',
         'emails': 'list<string>',
         'engagement': 'Engagement',
         'fan_count': 'unsigned int',
         'featured_video': 'AdVideo',
         'features': 'string',
+        'followers_count': 'unsigned int',
         'food_styles': 'list<string>',
         'founded': 'string',
         'general_info': 'string',
         'general_manager': 'string',
         'genre': 'string',
         'global_brand_page_name': 'string',
         'global_brand_root_id': 'string',
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/pageadminnote.py` & `facebook_business-9.0.3/facebook_business/adobjects/pageadminnote.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/pagecalltoaction.py` & `facebook_business-9.0.3/facebook_business/adobjects/pagecalltoaction.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,14 +66,15 @@
         become_a_volunteer = 'BECOME_A_VOLUNTEER'
         email = 'EMAIL'
         facebook_app = 'FACEBOOK_APP'
         follow = 'FOLLOW'
         marketplace_inventory_page = 'MARKETPLACE_INVENTORY_PAGE'
         messenger = 'MESSENGER'
         mini_shop = 'MINI_SHOP'
+        mobile_center = 'MOBILE_CENTER'
         none = 'NONE'
         phone_call = 'PHONE_CALL'
         shop_on_facebook = 'SHOP_ON_FACEBOOK'
         website = 'WEBSITE'
 
     class IphoneDestinationType:
         app_deeplink = 'APP_DEEPLINK'
@@ -104,14 +105,15 @@
         get_offer = 'GET_OFFER'
         get_offer_view = 'GET_OFFER_VIEW'
         interested = 'INTERESTED'
         learn_more = 'LEARN_MORE'
         listen = 'LISTEN'
         local_dev_platform = 'LOCAL_DEV_PLATFORM'
         message = 'MESSAGE'
+        mobile_center = 'MOBILE_CENTER'
         open_app = 'OPEN_APP'
         order_food = 'ORDER_FOOD'
         play_music = 'PLAY_MUSIC'
         play_now = 'PLAY_NOW'
         purchase_gift_cards = 'PURCHASE_GIFT_CARDS'
         request_appointment = 'REQUEST_APPOINTMENT'
         request_quote = 'REQUEST_QUOTE'
@@ -126,14 +128,15 @@
 
     class WebDestinationType:
         become_a_volunteer = 'BECOME_A_VOLUNTEER'
         become_supporter = 'BECOME_SUPPORTER'
         email = 'EMAIL'
         follow = 'FOLLOW'
         messenger = 'MESSENGER'
+        mobile_center = 'MOBILE_CENTER'
         none = 'NONE'
         shop_on_facebook = 'SHOP_ON_FACEBOOK'
         website = 'WEBSITE'
 
     def api_delete(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
         from facebook_business.utils import api_utils
         if batch is None and (success is not None or failure is not None):
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/pagecategory.py` & `facebook_business-9.0.3/facebook_business/adobjects/pagecategory.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/pagechangeproposal.py` & `facebook_business-9.0.3/facebook_business/adobjects/pagechangeproposal.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/pageparking.py` & `facebook_business-9.0.3/facebook_business/adobjects/pageparking.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/pagepaymentoptions.py` & `facebook_business-9.0.3/facebook_business/adobjects/pagepaymentoptions.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/pagepost.py` & `facebook_business-9.0.3/facebook_business/adobjects/pagepost.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/pagerestaurantservices.py` & `facebook_business-9.0.3/facebook_business/adobjects/pagerestaurantservices.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/pagerestaurantspecialties.py` & `facebook_business-9.0.3/facebook_business/adobjects/pagerestaurantspecialties.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/pagesavedfilter.py` & `facebook_business-9.0.3/facebook_business/adobjects/pagesavedfilter.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/pagesettings.py` & `facebook_business-9.0.3/facebook_business/adobjects/pagesettings.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/pagestartinfo.py` & `facebook_business-9.0.3/facebook_business/adobjects/pagestartinfo.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/pagethreadowner.py` & `facebook_business-9.0.3/facebook_business/adobjects/pagethreadowner.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/pageupcomingchange.py` & `facebook_business-9.0.3/facebook_business/adobjects/pageupcomingchange.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/pageusermessagethreadlabel.py` & `facebook_business-9.0.3/facebook_business/adobjects/pageusermessagethreadlabel.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/partnerstudy.py` & `facebook_business-9.0.3/facebook_business/adobjects/partnerstudy.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/paymentenginepayment.py` & `facebook_business-9.0.3/facebook_business/adobjects/paymentenginepayment.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/paymentpricepoints.py` & `facebook_business-9.0.3/facebook_business/adobjects/paymentpricepoints.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/paymentsubscription.py` & `facebook_business-9.0.3/facebook_business/adobjects/paymentsubscription.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/permission.py` & `facebook_business-9.0.3/facebook_business/adobjects/permission.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/persona.py` & `facebook_business-9.0.3/facebook_business/adobjects/persona.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/photo.py` & `facebook_business-9.0.3/facebook_business/adobjects/photo.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/place.py` & `facebook_business-9.0.3/facebook_business/adobjects/place.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/placetopic.py` & `facebook_business-9.0.3/facebook_business/adobjects/placetopic.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/platformimagesource.py` & `facebook_business-9.0.3/facebook_business/adobjects/platformimagesource.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/playablecontent.py` & `facebook_business-9.0.3/facebook_business/adobjects/playablecontent.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/post.py` & `facebook_business-9.0.3/facebook_business/adobjects/post.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/privacy.py` & `facebook_business-9.0.3/facebook_business/adobjects/privacy.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/productcatalog.py` & `facebook_business-9.0.3/facebook_business/adobjects/productcatalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,15 @@
         cameras = 'CAMERAS'
         cell_phones_and_smart_watches = 'CELL_PHONES_AND_SMART_WATCHES'
         cleaning_supplies = 'CLEANING_SUPPLIES'
         clothing = 'CLOTHING'
         clothing_accessories = 'CLOTHING_ACCESSORIES'
         computers_and_tablets = 'COMPUTERS_AND_TABLETS'
         diapering_and_potty_training = 'DIAPERING_AND_POTTY_TRAINING'
+        digital_product_offer = 'DIGITAL_PRODUCT_OFFER'
         electronics_accessories = 'ELECTRONICS_ACCESSORIES'
         furniture = 'FURNITURE'
         health = 'HEALTH'
         home_goods = 'HOME_GOODS'
         jewelry = 'JEWELRY'
         nursery = 'NURSERY'
         printers_and_scanners = 'PRINTERS_AND_SCANNERS'
@@ -463,14 +464,57 @@
             return request
         elif pending:
             return request
         else:
             self.assure_call()
             return request.execute()
 
+    def create_automotive_model(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
+        from facebook_business.utils import api_utils
+        if batch is None and (success is not None or failure is not None):
+          api_utils.warning('`success` and `failure` callback only work for batch call.')
+        from facebook_business.adobjects.automotivemodel import AutomotiveModel
+        param_types = {
+            'automotive_model_id': 'string',
+            'body_style': 'body_style_enum',
+            'currency': 'string',
+            'description': 'string',
+            'images': 'list<Object>',
+            'make': 'string',
+            'model': 'string',
+            'price': 'unsigned int',
+            'title': 'string',
+            'url': 'string',
+            'year': 'unsigned int',
+        }
+        enums = {
+            'body_style_enum': AutomotiveModel.BodyStyle.__dict__.values(),
+        }
+        request = FacebookRequest(
+            node_id=self['id'],
+            method='POST',
+            endpoint='/automotive_models',
+            api=self._api,
+            param_checker=TypeChecker(param_types, enums),
+            target_class=AutomotiveModel,
+            api_type='EDGE',
+            response_parser=ObjectParser(target_class=AutomotiveModel, api=self._api),
+        )
+        request.add_params(params)
+        request.add_fields(fields)
+
+        if batch is not None:
+            request.add_to_batch(batch, success=success, failure=failure)
+            return request
+        elif pending:
+            return request
+        else:
+            self.assure_call()
+            return request.execute()
+
     def create_batch(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
         from facebook_business.utils import api_utils
         if batch is None and (success is not None or failure is not None):
           api_utils.warning('`success` and `failure` callback only work for batch call.')
         param_types = {
             'allow_upsert': 'bool',
             'fbe_external_business_id': 'string',
@@ -1199,16 +1243,16 @@
             'migrated_from_feed_id': 'string',
             'name': 'string',
             'override_type': 'override_type_enum',
             'override_value': 'string',
             'quoted_fields_mode': 'quoted_fields_mode_enum',
             'rules': 'list<string>',
             'schedule': 'string',
+            'selected_override_fields': 'list<string>',
             'update_schedule': 'string',
-            'whitelisted_properties': 'list<string>',
         }
         enums = {
             'delimiter_enum': ProductFeed.Delimiter.__dict__.values(),
             'encoding_enum': ProductFeed.Encoding.__dict__.values(),
             'feed_type_enum': ProductFeed.FeedType.__dict__.values(),
             'item_sub_type_enum': ProductFeed.ItemSubType.__dict__.values(),
             'override_type_enum': ProductFeed.OverrideType.__dict__.values(),
@@ -1438,15 +1482,14 @@
 
     def create_product(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
         from facebook_business.utils import api_utils
         if batch is None and (success is not None or failure is not None):
           api_utils.warning('`success` and `failure` callback only work for batch call.')
         from facebook_business.adobjects.productitem import ProductItem
         param_types = {
-            'additional_image_files': 'list<file>',
             'additional_image_urls': 'list<string>',
             'additional_uploaded_image_ids': 'list<string>',
             'additional_variant_attributes': 'map',
             'android_app_name': 'string',
             'android_class': 'string',
             'android_package': 'string',
             'android_url': 'string',
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/productcatalogcategory.py` & `facebook_business-9.0.3/facebook_business/adobjects/productcatalogcategory.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/productcataloghotelroomsbatch.py` & `facebook_business-9.0.3/facebook_business/adobjects/productcataloghotelroomsbatch.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/productcatalogimagesettings.py` & `facebook_business-9.0.3/facebook_business/adobjects/productcatalogimagesettings.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/productcatalogimagesettingsoperation.py` & `facebook_business-9.0.3/facebook_business/adobjects/productcatalogimagesettingsoperation.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/productcatalogpricingvariablesbatch.py` & `facebook_business-9.0.3/facebook_business/adobjects/productcatalogpricingvariablesbatch.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/productcatalogproductsetsbatch.py` & `facebook_business-9.0.3/facebook_business/adobjects/productcatalogproductsetsbatch.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/producteventstat.py` & `facebook_business-9.0.3/facebook_business/adobjects/producteventstat.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/productfeed.py` & `facebook_business-9.0.3/facebook_business/adobjects/productfeed.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         product_count = 'product_count'
         quoted_fields_mode = 'quoted_fields_mode'
         schedule = 'schedule'
         update_schedule = 'update_schedule'
         feed_type = 'feed_type'
         override_value = 'override_value'
         rules = 'rules'
-        whitelisted_properties = 'whitelisted_properties'
+        selected_override_fields = 'selected_override_fields'
 
     class Delimiter:
         autodetect = 'AUTODETECT'
         bar = 'BAR'
         comma = 'COMMA'
         semicolon = 'SEMICOLON'
         tab = 'TAB'
@@ -110,14 +110,15 @@
         cameras = 'CAMERAS'
         cell_phones_and_smart_watches = 'CELL_PHONES_AND_SMART_WATCHES'
         cleaning_supplies = 'CLEANING_SUPPLIES'
         clothing = 'CLOTHING'
         clothing_accessories = 'CLOTHING_ACCESSORIES'
         computers_and_tablets = 'COMPUTERS_AND_TABLETS'
         diapering_and_potty_training = 'DIAPERING_AND_POTTY_TRAINING'
+        digital_product_offer = 'DIGITAL_PRODUCT_OFFER'
         electronics_accessories = 'ELECTRONICS_ACCESSORIES'
         furniture = 'FURNITURE'
         health = 'HEALTH'
         home_goods = 'HOME_GOODS'
         jewelry = 'JEWELRY'
         nursery = 'NURSERY'
         printers_and_scanners = 'PRINTERS_AND_SCANNERS'
@@ -725,15 +726,15 @@
         'product_count': 'int',
         'quoted_fields_mode': 'QuotedFieldsMode',
         'schedule': 'ProductFeedSchedule',
         'update_schedule': 'ProductFeedSchedule',
         'feed_type': 'FeedType',
         'override_value': 'string',
         'rules': 'list<string>',
-        'whitelisted_properties': 'list<string>',
+        'selected_override_fields': 'list<string>',
     }
     @classmethod
     def _get_field_enum_info(cls):
         field_enum_info = {}
         field_enum_info['Delimiter'] = ProductFeed.Delimiter.__dict__.values()
         field_enum_info['QuotedFieldsMode'] = ProductFeed.QuotedFieldsMode.__dict__.values()
         field_enum_info['Encoding'] = ProductFeed.Encoding.__dict__.values()
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/productfeedmissingfeeditemreplacement.py` & `facebook_business-9.0.3/facebook_business/adobjects/productfeedmissingfeeditemreplacement.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/productfeedrule.py` & `facebook_business-9.0.3/facebook_business/adobjects/productfeedrule.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/productfeedrulesuggestion.py` & `facebook_business-9.0.3/facebook_business/adobjects/productfeedrulesuggestion.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/productfeedschedule.py` & `facebook_business-9.0.3/facebook_business/adobjects/productfeedschedule.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/productfeedupload.py` & `facebook_business-9.0.3/facebook_business/adobjects/productfeedupload.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/productfeeduploaddiagnosticsreport.py` & `facebook_business-9.0.3/facebook_business/adobjects/productfeeduploaddiagnosticsreport.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/productfeeduploaderror.py` & `facebook_business-9.0.3/facebook_business/adobjects/productfeeduploaderror.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/productfeeduploaderrorreport.py` & `facebook_business-9.0.3/facebook_business/adobjects/productfeeduploaderrorreport.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/productfeeduploaderrorsample.py` & `facebook_business-9.0.3/facebook_business/adobjects/productfeeduploaderrorsample.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/productgroup.py` & `facebook_business-9.0.3/facebook_business/adobjects/productgroup.py`

 * *Files 4% similar despite different names*

```diff
@@ -144,58 +144,14 @@
             return request
         elif pending:
             return request
         else:
             self.assure_call()
             return request.execute()
 
-    def create_ar_datum(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
-        from facebook_business.utils import api_utils
-        if batch is None and (success is not None or failure is not None):
-          api_utils.warning('`success` and `failure` callback only work for batch call.')
-        param_types = {
-            'effect_icon': 'file',
-            'state': 'state_enum',
-            'surfaces': 'list<surfaces_enum>',
-        }
-        enums = {
-            'state_enum': [
-                'DISABLED',
-                'ENABLED',
-                'TEST',
-            ],
-            'surfaces_enum': [
-                'SHOPS',
-                'TEST_CAPABILITY',
-                'UNIVERSAL_CHECKOUT',
-                'US_MARKETPLACE',
-            ],
-        }
-        request = FacebookRequest(
-            node_id=self['id'],
-            method='POST',
-            endpoint='/ar_data',
-            api=self._api,
-            param_checker=TypeChecker(param_types, enums),
-            target_class=AbstractCrudObject,
-            api_type='EDGE',
-            response_parser=ObjectParser(target_class=AbstractCrudObject, api=self._api),
-        )
-        request.add_params(params)
-        request.add_fields(fields)
-
-        if batch is not None:
-            request.add_to_batch(batch, success=success, failure=failure)
-            return request
-        elif pending:
-            return request
-        else:
-            self.assure_call()
-            return request.execute()
-
     def get_products(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
         from facebook_business.utils import api_utils
         if batch is None and (success is not None or failure is not None):
           api_utils.warning('`success` and `failure` callback only work for batch call.')
         from facebook_business.adobjects.productitem import ProductItem
         param_types = {
         }
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/productitem.py` & `facebook_business-9.0.3/facebook_business/adobjects/productitem.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 
     class Field(AbstractObject.Field):
         additional_image_cdn_urls = 'additional_image_cdn_urls'
         additional_image_urls = 'additional_image_urls'
         additional_variant_attributes = 'additional_variant_attributes'
         age_group = 'age_group'
         applinks = 'applinks'
+        ar_data = 'ar_data'
         availability = 'availability'
         brand = 'brand'
         capability_to_review_status = 'capability_to_review_status'
         category = 'category'
         category_specific_fields = 'category_specific_fields'
         color = 'color'
         commerce_insights = 'commerce_insights'
@@ -93,15 +94,14 @@
         shipping_weight_unit = 'shipping_weight_unit'
         shipping_weight_value = 'shipping_weight_value'
         short_description = 'short_description'
         size = 'size'
         start_date = 'start_date'
         url = 'url'
         visibility = 'visibility'
-        additional_image_files = 'additional_image_files'
         additional_uploaded_image_ids = 'additional_uploaded_image_ids'
         android_app_name = 'android_app_name'
         android_class = 'android_class'
         android_package = 'android_package'
         android_url = 'android_url'
         checkout_url = 'checkout_url'
         commerce_tax_category = 'commerce_tax_category'
@@ -448,15 +448,14 @@
             return request.execute()
 
     def api_update(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
         from facebook_business.utils import api_utils
         if batch is None and (success is not None or failure is not None):
           api_utils.warning('`success` and `failure` callback only work for batch call.')
         param_types = {
-            'additional_image_files': 'list<file>',
             'additional_image_urls': 'list<string>',
             'additional_uploaded_image_ids': 'list<string>',
             'additional_variant_attributes': 'map',
             'android_app_name': 'string',
             'android_class': 'string',
             'android_package': 'string',
             'android_url': 'string',
@@ -542,50 +541,14 @@
             return request
         elif pending:
             return request
         else:
             self.assure_call()
             return request.execute()
 
-    def create_ar_datum(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
-        from facebook_business.utils import api_utils
-        if batch is None and (success is not None or failure is not None):
-          api_utils.warning('`success` and `failure` callback only work for batch call.')
-        param_types = {
-            'container_effect': 'container_effect_enum',
-            'effect_parameters': 'map',
-            'picker_icon': 'file',
-        }
-        enums = {
-            'container_effect_enum': [
-                'MAKEUP',
-            ],
-        }
-        request = FacebookRequest(
-            node_id=self['id'],
-            method='POST',
-            endpoint='/ar_data',
-            api=self._api,
-            param_checker=TypeChecker(param_types, enums),
-            target_class=AbstractCrudObject,
-            api_type='EDGE',
-            response_parser=ObjectParser(target_class=AbstractCrudObject, api=self._api),
-        )
-        request.add_params(params)
-        request.add_fields(fields)
-
-        if batch is not None:
-            request.add_to_batch(batch, success=success, failure=failure)
-            return request
-        elif pending:
-            return request
-        else:
-            self.assure_call()
-            return request.execute()
-
     def get_channels_to_integrity_status(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
         from facebook_business.utils import api_utils
         if batch is None and (success is not None or failure is not None):
           api_utils.warning('`success` and `failure` callback only work for batch call.')
         from facebook_business.adobjects.catalogitemchannelstointegritystatus import CatalogItemChannelsToIntegrityStatus
         param_types = {
         }
@@ -646,14 +609,15 @@
 
     _field_types = {
         'additional_image_cdn_urls': 'list<map<string, string>>',
         'additional_image_urls': 'list<string>',
         'additional_variant_attributes': 'map<string, string>',
         'age_group': 'AgeGroup',
         'applinks': 'CatalogItemAppLinks',
+        'ar_data': 'ProductItemARData',
         'availability': 'Availability',
         'brand': 'string',
         'capability_to_review_status': 'map<Object, Object>',
         'category': 'string',
         'category_specific_fields': 'CatalogSubVerticalList',
         'color': 'string',
         'commerce_insights': 'ProductItemCommerceInsights',
@@ -697,15 +661,14 @@
         'shipping_weight_unit': 'ShippingWeightUnit',
         'shipping_weight_value': 'float',
         'short_description': 'string',
         'size': 'string',
         'start_date': 'string',
         'url': 'string',
         'visibility': 'Visibility',
-        'additional_image_files': 'list<file>',
         'additional_uploaded_image_ids': 'list<string>',
         'android_app_name': 'string',
         'android_class': 'string',
         'android_package': 'string',
         'android_url': 'string',
         'checkout_url': 'string',
         'commerce_tax_category': 'CommerceTaxCategory',
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/productitemcommerceinsights.py` & `facebook_business-9.0.3/facebook_business/adobjects/productitemcommerceinsights.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/productset.py` & `facebook_business-9.0.3/facebook_business/adobjects/productset.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/productsetmetadata.py` & `facebook_business-9.0.3/facebook_business/adobjects/productsetmetadata.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/productvariant.py` & `facebook_business-9.0.3/facebook_business/adobjects/productvariant.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/profile.py` & `facebook_business-9.0.3/facebook_business/adobjects/profile.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/profilepicturesource.py` & `facebook_business-9.0.3/facebook_business/adobjects/profilepicturesource.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/publisherblocklist.py` & `facebook_business-9.0.3/facebook_business/adobjects/publisherblocklist.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/rawcustomaudience.py` & `facebook_business-9.0.3/facebook_business/adobjects/rawcustomaudience.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/reachfrequencyactivity.py` & `facebook_business-9.0.3/facebook_business/adobjects/reachfrequencyactivity.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/reachfrequencyadformat.py` & `facebook_business-9.0.3/facebook_business/adobjects/reachfrequencyadformat.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/reachfrequencycurvelowerconfidencerange.py` & `facebook_business-9.0.3/facebook_business/adobjects/reachfrequencycurvelowerconfidencerange.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/reachfrequencycurveupperconfidencerange.py` & `facebook_business-9.0.3/facebook_business/adobjects/reachfrequencycurveupperconfidencerange.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/reachfrequencydaypart.py` & `facebook_business-9.0.3/facebook_business/adobjects/reachfrequencydaypart.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/reachfrequencyestimatescurve.py` & `facebook_business-9.0.3/facebook_business/adobjects/reachfrequencyestimatescurve.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/reachfrequencyestimatesplacementbreakdown.py` & `facebook_business-9.0.3/facebook_business/adobjects/reachfrequencyestimatesplacementbreakdown.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/reachfrequencyprediction.py` & `facebook_business-9.0.3/facebook_business/adobjects/reachfrequencyprediction.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/reachfrequencyspec.py` & `facebook_business-9.0.3/facebook_business/adobjects/reachfrequencyspec.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/readonlyanalyticsuserpropertyconfig.py` & `facebook_business-9.0.3/facebook_business/adobjects/savedmessageresponse.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,25 +28,29 @@
 This class is auto-generated.
 
 For any issues or feature requests related to this class, please let us know on
 github and we'll fix in our codegen framework. We'll not be able to accept
 pull request for this class.
 """
 
-class ReadOnlyAnalyticsUserPropertyConfig(
+class SavedMessageResponse(
     AbstractCrudObject,
 ):
 
     def __init__(self, fbid=None, parent_id=None, api=None):
-        self._isReadOnlyAnalyticsUserPropertyConfig = True
-        super(ReadOnlyAnalyticsUserPropertyConfig, self).__init__(fbid, parent_id, api)
+        self._isSavedMessageResponse = True
+        super(SavedMessageResponse, self).__init__(fbid, parent_id, api)
 
     class Field(AbstractObject.Field):
-        active_properties = 'active_properties'
+        category = 'category'
         id = 'id'
+        image = 'image'
+        is_enabled = 'is_enabled'
+        message = 'message'
+        title = 'title'
 
     def api_get(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
         from facebook_business.utils import api_utils
         if batch is None and (success is not None or failure is not None):
           api_utils.warning('`success` and `failure` callback only work for batch call.')
         param_types = {
         }
@@ -54,15 +58,15 @@
         }
         request = FacebookRequest(
             node_id=self['id'],
             method='GET',
             endpoint='/',
             api=self._api,
             param_checker=TypeChecker(param_types, enums),
-            target_class=ReadOnlyAnalyticsUserPropertyConfig,
+            target_class=SavedMessageResponse,
             api_type='NODE',
             response_parser=ObjectParser(reuse_object=self),
         )
         request.add_params(params)
         request.add_fields(fields)
 
         if batch is not None:
@@ -71,16 +75,20 @@
         elif pending:
             return request
         else:
             self.assure_call()
             return request.execute()
 
     _field_types = {
-        'active_properties': 'list<string>',
+        'category': 'string',
         'id': 'string',
+        'image': 'string',
+        'is_enabled': 'bool',
+        'message': 'string',
+        'title': 'string',
     }
     @classmethod
     def _get_field_enum_info(cls):
         field_enum_info = {}
         return field_enum_info
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/recommendation.py` & `facebook_business-9.0.3/facebook_business/adobjects/recommendation.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/referral.py` & `facebook_business-9.0.3/facebook_business/adobjects/referral.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/revsharepolicy.py` & `facebook_business-9.0.3/facebook_business/adobjects/revsharepolicy.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/richmediaelement.py` & `facebook_business-9.0.3/facebook_business/adobjects/targetingproductaudiencesubspec.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,32 +24,30 @@
 This class is auto-generated.
 
 For any issues or feature requests related to this class, please let us know on
 github and we'll fix in our codegen framework. We'll not be able to accept
 pull request for this class.
 """
 
-class RichMediaElement(
+class TargetingProductAudienceSubSpec(
     AbstractObject,
 ):
 
     def __init__(self, api=None):
-        super(RichMediaElement, self).__init__()
-        self._isRichMediaElement = True
+        super(TargetingProductAudienceSubSpec, self).__init__()
+        self._isTargetingProductAudienceSubSpec = True
         self._api = api
 
     class Field(AbstractObject.Field):
-        element = 'element'
-        element_type = 'element_type'
-        name = 'name'
+        retention_seconds = 'retention_seconds'
+        rule = 'rule'
 
     _field_types = {
-        'element': 'Object',
-        'element_type': 'string',
-        'name': 'string',
+        'retention_seconds': 'string',
+        'rule': 'string',
     }
     @classmethod
     def _get_field_enum_info(cls):
         field_enum_info = {}
         return field_enum_info
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/rtbdynamicpost.py` & `facebook_business-9.0.3/facebook_business/adobjects/rtbdynamicpost.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/savedaudience.py` & `facebook_business-9.0.3/facebook_business/adobjects/savedaudience.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/savedmessageresponse.py` & `facebook_business-9.0.3/facebook_business/adobjects/videocopyrightrule.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,29 +28,35 @@
 This class is auto-generated.
 
 For any issues or feature requests related to this class, please let us know on
 github and we'll fix in our codegen framework. We'll not be able to accept
 pull request for this class.
 """
 
-class SavedMessageResponse(
+class VideoCopyrightRule(
     AbstractCrudObject,
 ):
 
     def __init__(self, fbid=None, parent_id=None, api=None):
-        self._isSavedMessageResponse = True
-        super(SavedMessageResponse, self).__init__(fbid, parent_id, api)
+        self._isVideoCopyrightRule = True
+        super(VideoCopyrightRule, self).__init__(fbid, parent_id, api)
 
     class Field(AbstractObject.Field):
-        category = 'category'
+        condition_groups = 'condition_groups'
+        copyrights = 'copyrights'
+        created_date = 'created_date'
+        creator = 'creator'
         id = 'id'
-        image = 'image'
-        is_enabled = 'is_enabled'
-        message = 'message'
-        title = 'title'
+        is_in_migration = 'is_in_migration'
+        name = 'name'
+
+    class Source:
+        match_settings_dialog = 'MATCH_SETTINGS_DIALOG'
+        rules_selector = 'RULES_SELECTOR'
+        rules_tab = 'RULES_TAB'
 
     def api_get(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
         from facebook_business.utils import api_utils
         if batch is None and (success is not None or failure is not None):
           api_utils.warning('`success` and `failure` callback only work for batch call.')
         param_types = {
         }
@@ -58,15 +64,15 @@
         }
         request = FacebookRequest(
             node_id=self['id'],
             method='GET',
             endpoint='/',
             api=self._api,
             param_checker=TypeChecker(param_types, enums),
-            target_class=SavedMessageResponse,
+            target_class=VideoCopyrightRule,
             api_type='NODE',
             response_parser=ObjectParser(reuse_object=self),
         )
         request.add_params(params)
         request.add_fields(fields)
 
         if batch is not None:
@@ -75,20 +81,22 @@
         elif pending:
             return request
         else:
             self.assure_call()
             return request.execute()
 
     _field_types = {
-        'category': 'string',
+        'condition_groups': 'list<VideoCopyrightConditionGroup>',
+        'copyrights': 'list<string>',
+        'created_date': 'datetime',
+        'creator': 'User',
         'id': 'string',
-        'image': 'string',
-        'is_enabled': 'bool',
-        'message': 'string',
-        'title': 'string',
+        'is_in_migration': 'bool',
+        'name': 'string',
     }
     @classmethod
     def _get_field_enum_info(cls):
         field_enum_info = {}
+        field_enum_info['Source'] = VideoCopyrightRule.Source.__dict__.values()
         return field_enum_info
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/securitysettings.py` & `facebook_business-9.0.3/facebook_business/adobjects/securitysettings.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/serverside/__init__.py` & `facebook_business-9.0.3/facebook_business/adobjects/serverside/__init__.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/serverside/action_source.py` & `facebook_business-9.0.3/facebook_business/adobjects/serverside/action_source.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/serverside/batch_processor.py` & `facebook_business-9.0.3/facebook_business/adobjects/serverside/batch_processor.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/serverside/content.py` & `facebook_business-9.0.3/facebook_business/adobjects/serverside/content.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/serverside/custom_data.py` & `facebook_business-9.0.3/facebook_business/adobjects/serverside/custom_data.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/serverside/delivery_category.py` & `facebook_business-9.0.3/facebook_business/adobjects/serverside/delivery_category.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/serverside/event.py` & `facebook_business-9.0.3/facebook_business/adobjects/serverside/event.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/serverside/event_request.py` & `facebook_business-9.0.3/facebook_business/adobjects/serverside/event_request.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/serverside/event_request_async.py` & `facebook_business-9.0.3/facebook_business/adobjects/serverside/event_request_async.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/serverside/event_response.py` & `facebook_business-9.0.3/facebook_business/adobjects/serverside/event_response.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/serverside/gender.py` & `facebook_business-9.0.3/facebook_business/adobjects/serverside/gender.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/serverside/http_method.py` & `facebook_business-9.0.3/facebook_business/adobjects/serverside/http_method.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/serverside/http_service_interface.py` & `facebook_business-9.0.3/facebook_business/adobjects/serverside/http_service_interface.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/serverside/normalize.py` & `facebook_business-9.0.3/facebook_business/adobjects/serverside/normalize.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/serverside/request_options.py` & `facebook_business-9.0.3/facebook_business/adobjects/serverside/request_options.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/serverside/tests/__init__.py` & `facebook_business-9.0.3/facebook_business/adobjects/serverside/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/serverside/tests/batch_processor_test.py` & `facebook_business-9.0.3/facebook_business/adobjects/serverside/tests/batch_processor_test.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/serverside/tests/content_test.py` & `facebook_business-9.0.3/facebook_business/adobjects/serverside/tests/content_test.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/serverside/tests/custom_data_test.py` & `facebook_business-9.0.3/facebook_business/adobjects/serverside/tests/custom_data_test.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/serverside/tests/event_request_async_test.py` & `facebook_business-9.0.3/facebook_business/adobjects/serverside/tests/event_request_async_test.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/serverside/tests/event_request_test.py` & `facebook_business-9.0.3/facebook_business/adobjects/serverside/tests/event_request_test.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/serverside/tests/event_test.py` & `facebook_business-9.0.3/facebook_business/adobjects/serverside/tests/event_test.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/serverside/tests/normalize_test.py` & `facebook_business-9.0.3/facebook_business/adobjects/serverside/tests/normalize_test.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/serverside/tests/user_data_test.py` & `facebook_business-9.0.3/facebook_business/adobjects/serverside/tests/user_data_test.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/serverside/tests/util_test.py` & `facebook_business-9.0.3/facebook_business/adobjects/serverside/tests/util_test.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/serverside/user_data.py` & `facebook_business-9.0.3/facebook_business/adobjects/serverside/user_data.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/serverside/util.py` & `facebook_business-9.0.3/facebook_business/adobjects/serverside/util.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/splittestwinner.py` & `facebook_business-9.0.3/facebook_business/adobjects/splittestwinner.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/storecatalogsettings.py` & `facebook_business-9.0.3/facebook_business/adobjects/storecatalogsettings.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/systemuser.py` & `facebook_business-9.0.3/facebook_business/adobjects/systemuser.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,14 +43,43 @@
     class Field(AbstractObject.Field):
         created_by = 'created_by'
         created_time = 'created_time'
         finance_permission = 'finance_permission'
         id = 'id'
         ip_permission = 'ip_permission'
         name = 'name'
+        role = 'role'
+        system_user_id = 'system_user_id'
+
+    class Role:
+        admin = 'ADMIN'
+        ads_rights_reviewer = 'ADS_RIGHTS_REVIEWER'
+        value_default = 'DEFAULT'
+        developer = 'DEVELOPER'
+        employee = 'EMPLOYEE'
+        finance_analyst = 'FINANCE_ANALYST'
+        finance_edit = 'FINANCE_EDIT'
+        finance_editor = 'FINANCE_EDITOR'
+        finance_view = 'FINANCE_VIEW'
+        manage = 'MANAGE'
+        partner_center_admin = 'PARTNER_CENTER_ADMIN'
+        partner_center_analyst = 'PARTNER_CENTER_ANALYST'
+        partner_center_education = 'PARTNER_CENTER_EDUCATION'
+        partner_center_marketing = 'PARTNER_CENTER_MARKETING'
+        partner_center_operations = 'PARTNER_CENTER_OPERATIONS'
+
+    # @deprecated get_endpoint function is deprecated
+    @classmethod
+    def get_endpoint(cls):
+        return 'system_users'
+
+    # @deprecated api_create is being deprecated
+    def api_create(self, parent_id, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
+        from facebook_business.adobjects.business import Business
+        return Business(api=self._api, fbid=parent_id).create_system_user(fields, params, batch, success, failure, pending)
 
     def api_get(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
         from facebook_business.utils import api_utils
         if batch is None and (success is not None or failure is not None):
           api_utils.warning('`success` and `failure` callback only work for batch call.')
         param_types = {
         }
@@ -206,14 +235,17 @@
     _field_types = {
         'created_by': 'User',
         'created_time': 'datetime',
         'finance_permission': 'string',
         'id': 'string',
         'ip_permission': 'string',
         'name': 'string',
+        'role': 'Role',
+        'system_user_id': 'int',
     }
     @classmethod
     def _get_field_enum_info(cls):
         field_enum_info = {}
+        field_enum_info['Role'] = SystemUser.Role.__dict__.values()
         return field_enum_info
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/tab.py` & `facebook_business-9.0.3/facebook_business/adobjects/tab.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/targeting.py` & `facebook_business-9.0.3/facebook_business/adobjects/targeting.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/targetingdynamicrule.py` & `facebook_business-9.0.3/facebook_business/adobjects/targetingdynamicrule.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/targetinggeolocation.py` & `facebook_business-9.0.3/facebook_business/adobjects/targetinggeolocation.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/targetinggeolocationcity.py` & `facebook_business-9.0.3/facebook_business/adobjects/targetinggeolocationcity.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/targetinggeolocationcustomlocation.py` & `facebook_business-9.0.3/facebook_business/adobjects/targetinggeolocationcustomlocation.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/targetinggeolocationelectoraldistrict.py` & `facebook_business-9.0.3/facebook_business/adobjects/targetinggeolocationelectoraldistrict.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/targetinggeolocationgeoentities.py` & `facebook_business-9.0.3/facebook_business/adobjects/targetinggeolocationgeoentities.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/targetinggeolocationlocationcluster.py` & `facebook_business-9.0.3/facebook_business/adobjects/targetinggeolocationlocationcluster.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/targetinggeolocationlocationexpansion.py` & `facebook_business-9.0.3/facebook_business/adobjects/targetinggeolocationlocationexpansion.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/targetinggeolocationmarket.py` & `facebook_business-9.0.3/facebook_business/adobjects/targetinggeolocationmarket.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/targetinggeolocationplace.py` & `facebook_business-9.0.3/facebook_business/adobjects/targetinggeolocationplace.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/targetinggeolocationpoliticaldistrict.py` & `facebook_business-9.0.3/facebook_business/adobjects/targetinggeolocationpoliticaldistrict.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/targetinggeolocationregion.py` & `facebook_business-9.0.3/facebook_business/adobjects/targetinggeolocationregion.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/targetinggeolocationzip.py` & `facebook_business-9.0.3/facebook_business/adobjects/targetinggeolocationzip.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/targetingproductaudiencespec.py` & `facebook_business-9.0.3/facebook_business/adobjects/targetingproductaudiencespec.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/targetingproductaudiencesubspec.py` & `facebook_business-9.0.3/facebook_business/adobjects/userleadgendisclaimerresponse.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,30 +24,30 @@
 This class is auto-generated.
 
 For any issues or feature requests related to this class, please let us know on
 github and we'll fix in our codegen framework. We'll not be able to accept
 pull request for this class.
 """
 
-class TargetingProductAudienceSubSpec(
+class UserLeadGenDisclaimerResponse(
     AbstractObject,
 ):
 
     def __init__(self, api=None):
-        super(TargetingProductAudienceSubSpec, self).__init__()
-        self._isTargetingProductAudienceSubSpec = True
+        super(UserLeadGenDisclaimerResponse, self).__init__()
+        self._isUserLeadGenDisclaimerResponse = True
         self._api = api
 
     class Field(AbstractObject.Field):
-        retention_seconds = 'retention_seconds'
-        rule = 'rule'
+        checkbox_key = 'checkbox_key'
+        is_checked = 'is_checked'
 
     _field_types = {
-        'retention_seconds': 'string',
-        'rule': 'string',
+        'checkbox_key': 'string',
+        'is_checked': 'string',
     }
     @classmethod
     def _get_field_enum_info(cls):
         field_enum_info = {}
         return field_enum_info
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/targetingprospectingaudience.py` & `facebook_business-9.0.3/facebook_business/adobjects/targetingprospectingaudience.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/targetingrelaxation.py` & `facebook_business-9.0.3/facebook_business/adobjects/targetingrelaxation.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/targetingsearch.py` & `facebook_business-9.0.3/facebook_business/adobjects/targetingsearch.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/targetingsentenceline.py` & `facebook_business-9.0.3/facebook_business/adobjects/targetingsentenceline.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/thirdpartymeasurementreportdataset.py` & `facebook_business-9.0.3/facebook_business/adobjects/thirdpartymeasurementreportdataset.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/trackingandconversionwithdefaults.py` & `facebook_business-9.0.3/facebook_business/adobjects/trackingandconversionwithdefaults.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/unifiedthread.py` & `facebook_business-9.0.3/facebook_business/adobjects/unifiedthread.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/url.py` & `facebook_business-9.0.3/facebook_business/adobjects/url.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/user.py` & `facebook_business-9.0.3/facebook_business/adobjects/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,14 +232,47 @@
             return request
         elif pending:
             return request
         else:
             self.assure_call()
             return request.execute()
 
+    def create_access_token(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
+        from facebook_business.utils import api_utils
+        if batch is None and (success is not None or failure is not None):
+          api_utils.warning('`success` and `failure` callback only work for batch call.')
+        param_types = {
+            'business_app': 'int',
+            'page_id': 'string',
+            'scope': 'list<Permission>',
+        }
+        enums = {
+        }
+        request = FacebookRequest(
+            node_id=self['id'],
+            method='POST',
+            endpoint='/access_tokens',
+            api=self._api,
+            param_checker=TypeChecker(param_types, enums),
+            target_class=User,
+            api_type='EDGE',
+            response_parser=ObjectParser(target_class=User, api=self._api),
+        )
+        request.add_params(params)
+        request.add_fields(fields)
+
+        if batch is not None:
+            request.add_to_batch(batch, success=success, failure=failure)
+            return request
+        elif pending:
+            return request
+        else:
+            self.assure_call()
+            return request.execute()
+
     def get_accounts(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
         from facebook_business.utils import api_utils
         if batch is None and (success is not None or failure is not None):
           api_utils.warning('`success` and `failure` callback only work for batch call.')
         from facebook_business.adobjects.page import Page
         param_types = {
             'is_place': 'bool',
@@ -837,14 +870,45 @@
             return request
         elif pending:
             return request
         else:
             self.assure_call()
             return request.execute()
 
+    def get_custom_labels(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
+        from facebook_business.utils import api_utils
+        if batch is None and (success is not None or failure is not None):
+          api_utils.warning('`success` and `failure` callback only work for batch call.')
+        from facebook_business.adobjects.pageusermessagethreadlabel import PageUserMessageThreadLabel
+        param_types = {
+        }
+        enums = {
+        }
+        request = FacebookRequest(
+            node_id=self['id'],
+            method='GET',
+            endpoint='/custom_labels',
+            api=self._api,
+            param_checker=TypeChecker(param_types, enums),
+            target_class=PageUserMessageThreadLabel,
+            api_type='EDGE',
+            response_parser=ObjectParser(target_class=PageUserMessageThreadLabel, api=self._api),
+        )
+        request.add_params(params)
+        request.add_fields(fields)
+
+        if batch is not None:
+            request.add_to_batch(batch, success=success, failure=failure)
+            return request
+        elif pending:
+            return request
+        else:
+            self.assure_call()
+            return request.execute()
+
     def get_events(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
         from facebook_business.utils import api_utils
         if batch is None and (success is not None or failure is not None):
           api_utils.warning('`success` and `failure` callback only work for batch call.')
         from facebook_business.adobjects.event import Event
         param_types = {
             'include_canceled': 'bool',
@@ -2046,15 +2110,14 @@
           api_utils.warning('`success` and `failure` callback only work for batch call.')
         from facebook_business.adobjects.advideo import AdVideo
         param_types = {
             'adaptive_type': 'string',
             'animated_effect_id': 'unsigned int',
             'application_id': 'string',
             'asked_fun_fact_prompt_id': 'unsigned int',
-            'attribution_app_id': 'string',
             'audio_story_wave_animation_handle': 'string',
             'composer_entry_picker': 'string',
             'composer_entry_point': 'string',
             'composer_entry_time': 'unsigned int',
             'composer_session_events_log': 'string',
             'composer_session_id': 'string',
             'composer_source_surface': 'string',
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/usercoverphoto.py` & `facebook_business-9.0.3/facebook_business/adobjects/usercoverphoto.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/userdevice.py` & `facebook_business-9.0.3/facebook_business/adobjects/userdevice.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/useridforapp.py` & `facebook_business-9.0.3/facebook_business/adobjects/useridforapp.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/useridforpage.py` & `facebook_business-9.0.3/facebook_business/adobjects/useridforpage.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/userleadgendisclaimerresponse.py` & `facebook_business-9.0.3/facebook_business/adobjects/videouploadlimits.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,30 +24,30 @@
 This class is auto-generated.
 
 For any issues or feature requests related to this class, please let us know on
 github and we'll fix in our codegen framework. We'll not be able to accept
 pull request for this class.
 """
 
-class UserLeadGenDisclaimerResponse(
+class VideoUploadLimits(
     AbstractObject,
 ):
 
     def __init__(self, api=None):
-        super(UserLeadGenDisclaimerResponse, self).__init__()
-        self._isUserLeadGenDisclaimerResponse = True
+        super(VideoUploadLimits, self).__init__()
+        self._isVideoUploadLimits = True
         self._api = api
 
     class Field(AbstractObject.Field):
-        checkbox_key = 'checkbox_key'
-        is_checked = 'is_checked'
+        length = 'length'
+        size = 'size'
 
     _field_types = {
-        'checkbox_key': 'string',
-        'is_checked': 'string',
+        'length': 'unsigned int',
+        'size': 'int',
     }
     @classmethod
     def _get_field_enum_info(cls):
         field_enum_info = {}
         return field_enum_info
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/userleadgenfielddata.py` & `facebook_business-9.0.3/facebook_business/adobjects/userleadgenfielddata.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/userpaymentmobilepricepoints.py` & `facebook_business-9.0.3/facebook_business/adobjects/userpaymentmobilepricepoints.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/valuebasedeligiblesource.py` & `facebook_business-9.0.3/facebook_business/adobjects/valuebasedeligiblesource.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/vehicle.py` & `facebook_business-9.0.3/facebook_business/adobjects/vehicle.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/vehicleoffer.py` & `facebook_business-9.0.3/facebook_business/adobjects/vehicleoffer.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/videocopyright.py` & `facebook_business-9.0.3/facebook_business/adobjects/videocopyright.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/videocopyrightconditiongroup.py` & `facebook_business-9.0.3/facebook_business/adobjects/videocopyrightconditiongroup.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/videocopyrightgeogate.py` & `facebook_business-9.0.3/facebook_business/adobjects/videocopyrightgeogate.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/videocopyrightrule.py` & `facebook_business-9.0.3/facebook_business/adobjects/whatsappbusinessprofile.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,35 +28,25 @@
 This class is auto-generated.
 
 For any issues or feature requests related to this class, please let us know on
 github and we'll fix in our codegen framework. We'll not be able to accept
 pull request for this class.
 """
 
-class VideoCopyrightRule(
+class WhatsAppBusinessProfile(
     AbstractCrudObject,
 ):
 
     def __init__(self, fbid=None, parent_id=None, api=None):
-        self._isVideoCopyrightRule = True
-        super(VideoCopyrightRule, self).__init__(fbid, parent_id, api)
+        self._isWhatsAppBusinessProfile = True
+        super(WhatsAppBusinessProfile, self).__init__(fbid, parent_id, api)
 
     class Field(AbstractObject.Field):
-        condition_groups = 'condition_groups'
-        copyrights = 'copyrights'
-        created_date = 'created_date'
-        creator = 'creator'
         id = 'id'
-        is_in_migration = 'is_in_migration'
-        name = 'name'
-
-    class Source:
-        match_settings_dialog = 'MATCH_SETTINGS_DIALOG'
-        rules_selector = 'RULES_SELECTOR'
-        rules_tab = 'RULES_TAB'
+        name_verification = 'name_verification'
 
     def api_get(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
         from facebook_business.utils import api_utils
         if batch is None and (success is not None or failure is not None):
           api_utils.warning('`success` and `failure` callback only work for batch call.')
         param_types = {
         }
@@ -64,15 +54,45 @@
         }
         request = FacebookRequest(
             node_id=self['id'],
             method='GET',
             endpoint='/',
             api=self._api,
             param_checker=TypeChecker(param_types, enums),
-            target_class=VideoCopyrightRule,
+            target_class=WhatsAppBusinessProfile,
+            api_type='NODE',
+            response_parser=ObjectParser(reuse_object=self),
+        )
+        request.add_params(params)
+        request.add_fields(fields)
+
+        if batch is not None:
+            request.add_to_batch(batch, success=success, failure=failure)
+            return request
+        elif pending:
+            return request
+        else:
+            self.assure_call()
+            return request.execute()
+
+    def api_update(self, fields=None, params=None, batch=None, success=None, failure=None, pending=False):
+        from facebook_business.utils import api_utils
+        if batch is None and (success is not None or failure is not None):
+          api_utils.warning('`success` and `failure` callback only work for batch call.')
+        param_types = {
+        }
+        enums = {
+        }
+        request = FacebookRequest(
+            node_id=self['id'],
+            method='POST',
+            endpoint='/',
+            api=self._api,
+            param_checker=TypeChecker(param_types, enums),
+            target_class=WhatsAppBusinessProfile,
             api_type='NODE',
             response_parser=ObjectParser(reuse_object=self),
         )
         request.add_params(params)
         request.add_fields(fields)
 
         if batch is not None:
@@ -81,22 +101,16 @@
         elif pending:
             return request
         else:
             self.assure_call()
             return request.execute()
 
     _field_types = {
-        'condition_groups': 'list<VideoCopyrightConditionGroup>',
-        'copyrights': 'list<string>',
-        'created_date': 'datetime',
-        'creator': 'User',
         'id': 'string',
-        'is_in_migration': 'bool',
-        'name': 'string',
+        'name_verification': 'Object',
     }
     @classmethod
     def _get_field_enum_info(cls):
         field_enum_info = {}
-        field_enum_info['Source'] = VideoCopyrightRule.Source.__dict__.values()
         return field_enum_info
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/videocopyrightsegment.py` & `facebook_business-9.0.3/facebook_business/adobjects/videocopyrightsegment.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/videolist.py` & `facebook_business-9.0.3/facebook_business/adobjects/videolist.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/videopoll.py` & `facebook_business-9.0.3/facebook_business/adobjects/videopoll.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/videothumbnail.py` & `facebook_business-9.0.3/facebook_business/adobjects/videothumbnail.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/videouploadlimits.py` & `facebook_business-9.0.3/facebook_business/adobjects/workuserfrontline.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,30 +24,30 @@
 This class is auto-generated.
 
 For any issues or feature requests related to this class, please let us know on
 github and we'll fix in our codegen framework. We'll not be able to accept
 pull request for this class.
 """
 
-class VideoUploadLimits(
+class WorkUserFrontline(
     AbstractObject,
 ):
 
     def __init__(self, api=None):
-        super(VideoUploadLimits, self).__init__()
-        self._isVideoUploadLimits = True
+        super(WorkUserFrontline, self).__init__()
+        self._isWorkUserFrontline = True
         self._api = api
 
     class Field(AbstractObject.Field):
-        length = 'length'
-        size = 'size'
+        has_access = 'has_access'
+        is_frontline = 'is_frontline'
 
     _field_types = {
-        'length': 'unsigned int',
-        'size': 'int',
+        'has_access': 'bool',
+        'is_frontline': 'bool',
     }
     @classmethod
     def _get_field_enum_info(cls):
         field_enum_info = {}
         return field_enum_info
```

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/voipinfo.py` & `facebook_business-9.0.3/facebook_business/adobjects/voipinfo.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/webapplink.py` & `facebook_business-9.0.3/facebook_business/adobjects/webapplink.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/whatsappbusinessaccount.py` & `facebook_business-9.0.3/facebook_business/adobjects/whatsappbusinessaccount.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/windowsapplink.py` & `facebook_business-9.0.3/facebook_business/adobjects/windowsapplink.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/windowsphoneapplink.py` & `facebook_business-9.0.3/facebook_business/adobjects/windowsphoneapplink.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/adobjects/workuserfrontline.py` & `facebook_business-9.0.3/facebook_business/adobjects/contextualbundlingspec.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,30 +24,28 @@
 This class is auto-generated.
 
 For any issues or feature requests related to this class, please let us know on
 github and we'll fix in our codegen framework. We'll not be able to accept
 pull request for this class.
 """
 
-class WorkUserFrontline(
+class ContextualBundlingSpec(
     AbstractObject,
 ):
 
     def __init__(self, api=None):
-        super(WorkUserFrontline, self).__init__()
-        self._isWorkUserFrontline = True
+        super(ContextualBundlingSpec, self).__init__()
+        self._isContextualBundlingSpec = True
         self._api = api
 
     class Field(AbstractObject.Field):
-        has_access = 'has_access'
-        is_frontline = 'is_frontline'
+        status = 'status'
 
     _field_types = {
-        'has_access': 'bool',
-        'is_frontline': 'bool',
+        'status': 'string',
     }
     @classmethod
     def _get_field_enum_info(cls):
         field_enum_info = {}
         return field_enum_info
```

### Comparing `facebook_business-9.0.2/facebook_business/api.py` & `facebook_business-9.0.3/facebook_business/api.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/apiconfig.py` & `facebook_business-9.0.3/facebook_business/apiconfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,10 +16,10 @@
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 ads_api_config = {
   'API_VERSION': 'v9.0',
-  'SDK_VERSION': 'v9.0.2',
+  'SDK_VERSION': 'v9.0.3',
   'STRICT_MODE': False
 }
```

### Comparing `facebook_business-9.0.2/facebook_business/bootstrap.py` & `facebook_business-9.0.3/facebook_business/bootstrap.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/crashreporter.py` & `facebook_business-9.0.3/facebook_business/crashreporter.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/docs_runner/doc_runner.py` & `facebook_business-9.0.3/facebook_business/docs_runner/doc_runner.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/docs_runner/get_version.py` & `facebook_business-9.0.3/facebook_business/docs_runner/get_version.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/exceptions.py` & `facebook_business-9.0.3/facebook_business/exceptions.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/exit_codes.py` & `facebook_business-9.0.3/facebook_business/exit_codes.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/fb_ca_chain_bundle.crt` & `facebook_business-9.0.3/facebook_business/fb_ca_chain_bundle.crt`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/mixins.py` & `facebook_business-9.0.3/facebook_business/mixins.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/session.py` & `facebook_business-9.0.3/facebook_business/session.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/specs.py` & `facebook_business-9.0.3/facebook_business/specs.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/test/docs.py` & `facebook_business-9.0.3/facebook_business/test/docs.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/test/docs_utils.py` & `facebook_business-9.0.3/facebook_business/test/docs_utils.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/test/integration_ad.py` & `facebook_business-9.0.3/facebook_business/test/integration_ad.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/test/integration_adaccount.py` & `facebook_business-9.0.3/facebook_business/test/integration_adaccount.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/test/integration_adcreative.py` & `facebook_business-9.0.3/facebook_business/test/integration_adcreative.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/test/integration_adset.py` & `facebook_business-9.0.3/facebook_business/test/integration_adset.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/test/integration_campaign.py` & `facebook_business-9.0.3/facebook_business/test/integration_campaign.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/test/integration_constant.py` & `facebook_business-9.0.3/facebook_business/test/integration_constant.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/test/integration_test_runner.py` & `facebook_business-9.0.3/facebook_business/test/integration_test_runner.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/test/integration_utils.py` & `facebook_business-9.0.3/facebook_business/test/integration_utils.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/test/misc/image.png` & `facebook_business-9.0.3/facebook_business/test/misc/image.png`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/test/other_docs.py` & `facebook_business-9.0.3/facebook_business/test/other_docs.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/test/test.png` & `facebook_business-9.0.3/facebook_business/test/test.png`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/test/unit.py` & `facebook_business-9.0.3/facebook_business/test/unit.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/typechecker.py` & `facebook_business-9.0.3/facebook_business/typechecker.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/utils/api_utils.py` & `facebook_business-9.0.3/facebook_business/utils/api_utils.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/utils/urls.py` & `facebook_business-9.0.3/facebook_business/utils/urls.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/utils/version.py` & `facebook_business-9.0.3/facebook_business/utils/version.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business/video_uploader.py` & `facebook_business-9.0.3/facebook_business/video_uploader.py`

 * *Files identical despite different names*

### Comparing `facebook_business-9.0.2/facebook_business.egg-info/PKG-INFO` & `facebook_business-9.0.3/facebook_business.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: facebook-business
-Version: 9.0.2
+Version: 9.0.3
 Summary: Facebook Business SDK
 Home-page: https://github.com/facebook/facebook-python-business-sdk
 Author: Facebook
 Author-email: 
 License: LICENSE.txt
-Download-URL: https://github.com/facebook/facebook-python-business-sdk/tarball/9.0.2
+Download-URL: https://github.com/facebook/facebook-python-business-sdk/tarball/9.0.3
 Description: # Facebook Business SDK for Python
         
         [![Build Status](https://travis-ci.org/facebook/facebook-python-business-sdk.svg)](https://travis-ci.org/facebook/facebook-python-business-sdk)
         
         ### Introduction
         
         The Facebook <a href="https://developers.facebook.com/docs/business-sdk" target="_blank">Business SDK</a> is a one-stop shop to help our partners better serve their businesses. Partners are using multiple Facebook API's to server the needs of their clients. Adopting all these API's and keeping them up to date across the various platforms can be time consuming and ultimately prohibitive. For this reason Facebook has developed the Business SDK bundling many of its APIs into one SDK to ease implementation and upkeep. The Business SDK is an upgraded version of the Marketing API SDK that includes the Marketing API as well as many Facebook APIs from different platforms such as Pages, Business Manager, Instagram, etc.
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: facebook-business Version: 9.0.2 Summary: Facebook
+Metadata-Version: 2.1 Name: facebook-business Version: 9.0.3 Summary: Facebook
 Business SDK Home-page: https://github.com/facebook/facebook-python-business-
 sdk Author: Facebook Author-email: License: LICENSE.txt Download-URL: https://
-github.com/facebook/facebook-python-business-sdk/tarball/9.0.2 Description: #
+github.com/facebook/facebook-python-business-sdk/tarball/9.0.3 Description: #
 Facebook Business SDK for Python [![Build Status](https://travis-ci.org/
 facebook/facebook-python-business-sdk.svg)](https://travis-ci.org/facebook/
 facebook-python-business-sdk) ### Introduction The Facebook Business_SDK is a
 one-stop shop to help our partners better serve their businesses. Partners are
 using multiple Facebook API's to server the needs of their clients. Adopting
 all these API's and keeping them up to date across the various platforms can be
 time consuming and ultimately prohibitive. For this reason Facebook has
```

### Comparing `facebook_business-9.0.2/facebook_business.egg-info/SOURCES.txt` & `facebook_business-9.0.3/facebook_business.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,14 @@
 facebook_business/adobjects/adaccountdefaultobjective.py
 facebook_business/adobjects/adaccountdeliveryestimate.py
 facebook_business/adobjects/adaccountmatchedsearchapplicationsedgedata.py
 facebook_business/adobjects/adaccountmaxbid.py
 facebook_business/adobjects/adaccountpromotableobjects.py
 facebook_business/adobjects/adaccountreachestimate.py
 facebook_business/adobjects/adaccountrecommendedcamapaignbudget.py
-facebook_business/adobjects/adaccountroas.py
 facebook_business/adobjects/adaccountsubscribedapps.py
 facebook_business/adobjects/adaccounttargetingunified.py
 facebook_business/adobjects/adaccounttrackingdata.py
 facebook_business/adobjects/adaccountuser.py
 facebook_business/adobjects/adactivity.py
 facebook_business/adobjects/adassetfeedspec.py
 facebook_business/adobjects/adassetfeedspecassetlabel.py
@@ -360,14 +359,15 @@
 facebook_business/adobjects/commercemerchantsettingssetupstatus.py
 facebook_business/adobjects/commerceorder.py
 facebook_business/adobjects/commerceordertransactiondetail.py
 facebook_business/adobjects/commercepayout.py
 facebook_business/adobjects/commercesettings.py
 facebook_business/adobjects/connectionstargeting.py
 facebook_business/adobjects/contentdeliveryreport.py
+facebook_business/adobjects/contextualbundlingspec.py
 facebook_business/adobjects/conversionactionquery.py
 facebook_business/adobjects/copyrightreferencecontainer.py
 facebook_business/adobjects/coverphoto.py
 facebook_business/adobjects/cpasadvertiserpartnershiprecommendation.py
 facebook_business/adobjects/cpascollaborationrequest.py
 facebook_business/adobjects/cpasparentcatalogsettings.py
 facebook_business/adobjects/creativehistory.py
@@ -413,14 +413,15 @@
 facebook_business/adobjects/homelisting.py
 facebook_business/adobjects/hotel.py
 facebook_business/adobjects/hotelroom.py
 facebook_business/adobjects/idname.py
 facebook_business/adobjects/igcomment.py
 facebook_business/adobjects/igmedia.py
 facebook_business/adobjects/iguser.py
+facebook_business/adobjects/imagecopyright.py
 facebook_business/adobjects/insightsresult.py
 facebook_business/adobjects/instagraminsightsresult.py
 facebook_business/adobjects/instagraminsightsvalue.py
 facebook_business/adobjects/instagramuser.py
 facebook_business/adobjects/instantarticle.py
 facebook_business/adobjects/instantarticleinsightsqueryresult.py
 facebook_business/adobjects/invoicecampaign.py
@@ -464,14 +465,15 @@
 facebook_business/adobjects/oracletransaction.py
 facebook_business/adobjects/outcomepredictionpoint.py
 facebook_business/adobjects/page.py
 facebook_business/adobjects/pageadminnote.py
 facebook_business/adobjects/pagecalltoaction.py
 facebook_business/adobjects/pagecategory.py
 facebook_business/adobjects/pagechangeproposal.py
+facebook_business/adobjects/pagecommerceeligibility.py
 facebook_business/adobjects/pageparking.py
 facebook_business/adobjects/pagepaymentoptions.py
 facebook_business/adobjects/pagepost.py
 facebook_business/adobjects/pagerestaurantservices.py
 facebook_business/adobjects/pagerestaurantspecialties.py
 facebook_business/adobjects/pagesavedfilter.py
 facebook_business/adobjects/pagesettings.py
@@ -508,14 +510,15 @@
 facebook_business/adobjects/productfeedupload.py
 facebook_business/adobjects/productfeeduploaddiagnosticsreport.py
 facebook_business/adobjects/productfeeduploaderror.py
 facebook_business/adobjects/productfeeduploaderrorreport.py
 facebook_business/adobjects/productfeeduploaderrorsample.py
 facebook_business/adobjects/productgroup.py
 facebook_business/adobjects/productitem.py
+facebook_business/adobjects/productitemardata.py
 facebook_business/adobjects/productitemcommerceinsights.py
 facebook_business/adobjects/productset.py
 facebook_business/adobjects/productsetmetadata.py
 facebook_business/adobjects/productvariant.py
 facebook_business/adobjects/profile.py
 facebook_business/adobjects/profilepicturesource.py
 facebook_business/adobjects/publisherblocklist.py
@@ -525,15 +528,14 @@
 facebook_business/adobjects/reachfrequencycurvelowerconfidencerange.py
 facebook_business/adobjects/reachfrequencycurveupperconfidencerange.py
 facebook_business/adobjects/reachfrequencydaypart.py
 facebook_business/adobjects/reachfrequencyestimatescurve.py
 facebook_business/adobjects/reachfrequencyestimatesplacementbreakdown.py
 facebook_business/adobjects/reachfrequencyprediction.py
 facebook_business/adobjects/reachfrequencyspec.py
-facebook_business/adobjects/readonlyanalyticsuserpropertyconfig.py
 facebook_business/adobjects/recommendation.py
 facebook_business/adobjects/referral.py
 facebook_business/adobjects/revsharepolicy.py
 facebook_business/adobjects/richmediaelement.py
 facebook_business/adobjects/rtbdynamicpost.py
 facebook_business/adobjects/savedaudience.py
 facebook_business/adobjects/savedmessageresponse.py
```

### Comparing `facebook_business-9.0.2/setup.py` & `facebook_business-9.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import os
 
 this_dir = os.path.dirname(__file__)
 readme_filename = os.path.join(this_dir, 'README.md')
 requirements_filename = os.path.join(this_dir, 'requirements.txt')
 
 PACKAGE_NAME = 'facebook_business'
-PACKAGE_VERSION = '9.0.2'
+PACKAGE_VERSION = '9.0.3'
 PACKAGE_AUTHOR = 'Facebook'
 PACKAGE_AUTHOR_EMAIL = ''
 PACKAGE_URL = 'https://github.com/facebook/facebook-python-business-sdk'
 PACKAGE_DOWNLOAD_URL = \
     'https://github.com/facebook/facebook-python-business-sdk/tarball/' + PACKAGE_VERSION
 PACKAGES = [
     'facebook_business',
```

