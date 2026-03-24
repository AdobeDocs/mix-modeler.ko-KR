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

![](/help/assets/icons/FileData.svg)**[!UICONTROL Models]****[!UICONTROL Open model canvas]**

## 설정

**[!UICONTROL Setup]**

1. **[!UICONTROL Name]**`Demo model`**[!UICONTROL Description]**`Demo model to explore AI features of Mix Modeler`

   ![](/help/assets/model-name-description.png)

1. **[!UICONTROL Next]****[!UICONTROL Cancel]**

## 구성{#configure}

>[!CONTEXTUALHELP]
>id="model_marketingtouchpoints_select"
>title="마케팅 접점"
>abstract="마케팅 접점이란 마케팅 투자가 미치는 숫자 또는 수익 기반 영향을 평가하는 데 사용되는 수신자, 개인 및/또는 쿠키 수준 마케팅 이벤트입니다.<br/><br/>겹치는 데이터가 있는 접점으로는 모델을 설정할 수 없으며 지출이 발생하는 점점이 최소 한 개 필요합니다."

**[!UICONTROL Configure]**

1. **[!UICONTROL Conversion goal]**

   ![](/help/assets/model-conversion-step.png)

   1. **[!UICONTROL Conversion]**[](../harmonize-data/conversions.md)[!UICONTROL Harmonized datasets]&#x200B;예: **[!UICONTROL Online Conversion]**.

   1. ![](/help/assets/icons/LinkOutLight.svg)**[!UICONTROL Create a conversion]**



1. **[!UICONTROL Marketing touchpoints]**[](../harmonize-data/marketing-touchpoints.md)[!UICONTROL Harmonized datasets]


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

         1. **[!UICONTROL equals]****[!UICONTROL not equals]****[!UICONTROL less than]****[!UICONTROL greater than]****[!UICONTROL starts with]****[!UICONTROL doesn't start with]****[!UICONTROL ends with]****[!UICONTROL doesn't end with]****[!UICONTROL contains]****[!UICONTROL doesn't contain]****[!UICONTROL is in]****[!UICONTROL is not in]**

         1. **[!UICONTROL __]**

      1. ![](/help/assets/icons/AddCircle.svg)**[!UICONTROL Add event]**

      1. ![](/help/assets/icons/CrossSize75.svg)

      1. **[!UICONTROL Any of]****[!UICONTROL All of]****[!UICONTROL Include ... Or ...]****[!UICONTROL Include ... And ...]**

   * ![](/help/assets/icons/AddCircle.svg)**[!UICONTROL Add eligible population]**

   * ![](/help/assets/icons/More.svg)**[!UICONTROL Remove container]**

   * ********

1. **[!UICONTROL Factor dataset]**

   ![](../assets/model-factors-dataset-step.png)

   * **[!UICONTROL Add Factor]**

      1. **[!UICONTROL Factor dataset]**[](/help/harmonize-data/dataset-rules.md#create-a-dataset-rule)[!UICONTROL Factor type**]**[!UICONTROL Internal]****[!UICONTROL External]**

      1. **[!UICONTROL Impact on conversion]****[!UICONTROL Auto]****[!UICONTROL Positive]****[!UICONTROL Negative]****[!UICONTROL Auto]**

   * ![](/help/assets/icons/CrossSize400.svg)




1. `1``52`**[!UICONTROL Give contribution credit to touchpoints occurring within]****[!UICONTROL weeks prior to the conversion]****[!UICONTROL Define lookback window]**

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

   * **[!UICONTROL MTA enabled]**[](insights.md#attribution)[](insights.md)

1. **[!UICONTROL Prior knowledge]**

   ![](/help/assets/model-prior-knowledge-step.png)

   1. **[!UICONTROL Rule type]****[!UICONTROL Absolute values]**

   1. **[!UICONTROL Name]****[!UICONTROL Contribution proportion]**

   1. **[!UICONTROL Level of confidence]**

   1. **[!UICONTROL Clear all]****[!UICONTROL Contribution proportion]****[!UICONTROL Level of confidence]**


## Set options

[](#schedule)[](#training-window)[](#granular-insights-reporting-fields)**[!UICONTROL Set options]**


### 일정

**[!UICONTROL Schedule]**

![](../assets/model-schedule.png)

To scheduled model scoring and training:

1. **[!UICONTROL Enable scheduled model scoring and training]**
1. **[!UICONTROL Scoring frequency]**

   * **[!UICONTROL Daily]**`05:22 pm`![](/help/assets/icons/Clock.svg)
   * **[!UICONTROL Weekly]**`05:22 pm`![](/help/assets/icons/Clock.svg)
   * **[!UICONTROL Monthly]**`05:22 pm`![](/help/assets/icons/Clock.svg)

1. **[!UICONTROL Training frequency]****[!UICONTROL Monthly]****[!UICONTROL Quarterly]****[!UICONTROL Yearly]****[!UICONTROL None]**


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

1. **[!UICONTROL __]****[!UICONTROL Includes]**
1. **[!UICONTROL **]**![](/help/assets/icons/CrossSize100.svg)
1. **[!UICONTROL Clear all]**

[](/help/ingest-data/schemas.md)[](/help/ingest-data/datasets.md)**[!UICONTROL conversionPassthrough]****[!UICONTROL touchpointPassthrough]**

![](/help/assets/schema-granular-insights-reporting.png)


## Finish

* **[!UICONTROL Finish]**

   * **[!UICONTROL Create instance?]****[!UICONTROL Ok]**![](/help/assets/icons/StatusOrange.svg)**[!UICONTROL Awaiting training]**

     **[!UICONTROL Cancel]**

   * If more configuration is needed, a red outline and text explains what additional configuration is required.

* **[!UICONTROL Back]**

* **[!UICONTROL Cancel]**

