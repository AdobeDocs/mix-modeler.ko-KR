---
title: Build models In Mix Modeler
description: Learn how to build models in Mix Modeler including how to set up, configure, and specify advanced options for the model.
feature: Models
solution: Mix Modeler
exl-id: e1093c09-1e23-460b-92de-cfb0061112fd
source-git-commit: 56682fb57d6ca99fbf5d355ae487af2b31a72319
workflow-type: tm+mt
source-wordcount: '1204'
ht-degree: 4%

---

# Build models

To build your custom AI-powered models, the interface provides a step-by-step guided model configuration flow.

![](/help/assets/icons/FileData.svg)**[!UICONTROL Models]**&#x200B;**[!UICONTROL Open model canvas]**

## 설정

**[!UICONTROL Setup]**

1. **[!UICONTROL Name]**`Demo model`**[!UICONTROL Description]**`Demo model to explore AI features of Mix Modeler`

   ![](/help/assets/model-name-description.png)

1. **[!UICONTROL Next]**&#x200B;**[!UICONTROL Cancel]**

## 구성{#configure}

>[!CONTEXTUALHELP]
>id="model_marketingtouchpoints_select"
>title="마케팅 접점"
>abstract="마케팅 접점이란 마케팅 투자가 미치는 숫자 또는 수익 기반 영향을 평가하는 데 사용되는 수신자, 개인 및/또는 쿠키 수준 마케팅 이벤트입니다.<br/><br/>겹치는 데이터가 있는 접점으로는 모델을 설정할 수 없으며 지출이 발생하는 점점이 최소 한 개 필요합니다."

**[!UICONTROL Configure]**

1. **[!UICONTROL Conversion goal]**

   ![](/help/assets/model-conversion-step.png)

   1. **[!UICONTROL Conversion]**&#x200B;[&#128279;](../harmonize-data/conversions.md) [!UICONTROL Harmonized datasets]&#x200B;예: **[!UICONTROL Online Conversion]**.

   1. ![](/help/assets/icons/LinkOutLight.svg)**[!UICONTROL Create a conversion]**



1. **[!UICONTROL Marketing touchpoints]**&#x200B;[&#128279;](../harmonize-data/marketing-touchpoints.md) [!UICONTROL Harmonized datasets]


   ![](/help/assets/model-marketing-touchpoint-step.png)

   1. **[!UICONTROL Touchpoint include]**

      * ![](/help/assets/icons/CrossSize75.svg)
      * **[!UICONTROL Clear all]**

   1. ![](/help/assets/icons/LinkOutLight.svg)**[!UICONTROL Create a touchpoint]**

   >[!NOTE]
   >
   >You cannot set up the model with touchpoints that have overlapping data and there must be at least one touchpoint with spend.

1. **[!UICONTROL Eligible data population]**

   ![](/help/assets/model-eligible-data-population-step.png)

   * For each container, define one or more events.

      1. For each event:

         1. **[!UICONTROL __]**

         1. **[!UICONTROL equals]**&#x200B;**[!UICONTROL not equals]**&#x200B;**[!UICONTROL less than]**&#x200B;**[!UICONTROL greater than]**&#x200B;**[!UICONTROL starts with]**&#x200B;**[!UICONTROL doesn't start with]**&#x200B;**[!UICONTROL ends with]**&#x200B;**[!UICONTROL doesn't end with]**&#x200B;**[!UICONTROL contains]**&#x200B;**[!UICONTROL doesn't contain]**&#x200B;**[!UICONTROL is in]**&#x200B;**[!UICONTROL is not in]**

         1. **[!UICONTROL __]**

      1. ![](/help/assets/icons/AddCircle.svg)**[!UICONTROL Add event]**

      1. ![](/help/assets/icons/CrossSize75.svg)

      1. **[!UICONTROL Any of]**&#x200B;**[!UICONTROL All of]**&#x200B;**[!UICONTROL Include ... Or ...]**&#x200B;**[!UICONTROL Include ... And ...]**

   * ![](/help/assets/icons/AddCircle.svg)**[!UICONTROL Add eligible population]**

   * ![](/help/assets/icons/More.svg)**[!UICONTROL Remove container]**

   * **&#x200B;**&#x200B;**&#x200B;**

1. **[!UICONTROL Factor dataset]**

   ![](../assets/model-factors-dataset-step.png)

   * **[!UICONTROL Add Factor]**

      1. **[!UICONTROL Factor dataset]**&#x200B;[&#128279;](/help/harmonize-data/dataset-rules.md#create-a-dataset-rule) [!UICONTROL Factor type&#x200B;**]**&#x200B;[!UICONTROL Internal]&#x200B;**&#x200B;**&#x200B;[!UICONTROL External]**

      1. **[!UICONTROL Impact on conversion]**&#x200B;**[!UICONTROL Auto]**&#x200B;**[!UICONTROL Positive]**&#x200B;**[!UICONTROL Negative]**&#x200B;**[!UICONTROL Auto]**

   * ![](/help/assets/icons/CrossSize400.svg)




1. `1` `52`**[!UICONTROL Give contribution credit to touchpoints occurring within]**&#x200B;**[!UICONTROL weeks prior to the conversion]**&#x200B;**[!UICONTROL Define lookback window]**

1. **[!UICONTROL Next]**<br/>**[!UICONTROL Back]**<br/>**[!UICONTROL Cancel]**


## 고급

**[!UICONTROL Advanced]**

1. **[!UICONTROL Spend share]**

   * **[!UICONTROL Allow spend share]**
      * A channel doesn&#39;t have enough observations (for example, low frequency of spend, impressions or clicks).
      * You are modeling spiky but regular, and potentially high-spend media (like TV for some brands), where data may be sparse.

     >[!NOTE]
     >
     >For one-off investments (for example a Super Bowl ad), consider to incorporate that data as a factor rather than to rely on spend share.
     >


1. **[!UICONTROL MTA enabled]**

   * **[!UICONTROL MTA enabled]**&#x200B;[&#128279;](insights.md#attribution) [&#128279;](insights.md)

1. **[!UICONTROL Prior knowledge]**

   ![](/help/assets/model-prior-knowledge-step.png)

   1. **[!UICONTROL Rule type]**&#x200B;**[!UICONTROL Absolute values]**

   1. **[!UICONTROL Name]**&#x200B;**[!UICONTROL Contribution proportion]**

   1. **[!UICONTROL Level of confidence]**

   1. **[!UICONTROL Clear all]**&#x200B;**[!UICONTROL Contribution proportion]**&#x200B;**[!UICONTROL Level of confidence]**


## Set options

[&#128279;](#schedule) [&#128279;](#training-window) [&#128279;](#granular-insights-reporting-fields)**[!UICONTROL Set options]**


### 일정

**[!UICONTROL Schedule]**

![](../assets/model-schedule.png)

To scheduled model scoring and training:

1. **[!UICONTROL Enable scheduled model scoring and training]**
1. **[!UICONTROL Scoring frequency]**

   * **[!UICONTROL Daily]**`05:22 pm`![](/help/assets/icons/Clock.svg)
   * **[!UICONTROL Weekly]**`05:22 pm`![](/help/assets/icons/Clock.svg)
   * **[!UICONTROL Monthly]**`05:22 pm`![](/help/assets/icons/Clock.svg)

1. **[!UICONTROL Training frequency]**&#x200B;**[!UICONTROL Monthly]**&#x200B;**[!UICONTROL Quarterly]**&#x200B;**[!UICONTROL Yearly]**&#x200B;**[!UICONTROL None]**


### Training window

**[!UICONTROL Define training window]**

![](/help/assets/model-define-training-window.png)

* **[!UICONTROL Have Mix Modeler select a helpful training window]**

* **[!UICONTROL Manually input a training window]**. **[!UICONTROL Include events the following years prior to a conversion]**


### Granular insights reporting fields

**[!UICONTROL Granular insights reporting fields]**

![](/help/assets/granular-insights-reporting-fields.png)

You define these harmonized fields so you can drill down in the reporting of your model using granular reporting columns instead of having to create separate models.

For example, you build a model that is focused on revenue, but you are also interested in the campaigns, media types, regions, and traffic sources performance. Without the granular incrementality reporting functionality, you would have to build four separate models. With the granular incrementality reporting functionality, you can break down your revenue model on campaigns, media types, regions, and traffic sources.

1. **[!UICONTROL __]**&#x200B;**[!UICONTROL Includes]**
1. **[!UICONTROL **]**![](/help/assets/icons/CrossSize100.svg)
1. **[!UICONTROL Clear all]**

[&#128279;](/help/ingest-data/schemas.md) [&#128279;](/help/ingest-data/datasets.md)**[!UICONTROL conversionPassthrough]**&#x200B;**[!UICONTROL touchpointPassthrough]**

![](/help/assets/schema-granular-insights-reporting.png)


## Finish

* **[!UICONTROL Finish]**

   * **[!UICONTROL Create instance?]**&#x200B;**[!UICONTROL Ok]**![](/help/assets/icons/StatusOrange.svg)**[!UICONTROL Awaiting training]**

     **[!UICONTROL Cancel]**

   * If more configuration is needed, a red outline and text explains what additional configuration is required.

* **[!UICONTROL Back]**

* **[!UICONTROL Cancel]**

