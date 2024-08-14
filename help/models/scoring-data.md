---
title: 채점 데이터
description: Mix Modeler에서 모델의 채점 데이터가 어떻게 지속되는지 알아봅니다.
feature: Models
exl-id: 2f2c3d20-7b14-41cc-a11a-03e8ad9e5d7a
source-git-commit: b6045176e82b97f848113f4e0ffbbb995c48b3d4
workflow-type: tm+mt
source-wordcount: '675'
ht-degree: 6%

---

# 채점 데이터

모델에 대한 채점을 수행하는 과정에서 채점 데이터는 Experience Platform의 데이터 세트 내에서 유지됩니다. 모델을 만드는 동안 다중 터치 속성을 활성화하면 추가 이벤트 점수 데이터가 Experience Platform의 데이터 세트 내에서 지속됩니다.

이러한 각 데이터 세트는 스키마를 준수합니다. 이 문서에서는 이러한 스키마를 설명합니다.


## 집계 채점 데이터 스키마

채점 데이터에 대한 스키마의 이름은 `AMM AI Schema - <name of model> <id>`과(와) 같이 지정됩니다. 예: `AMM AI Schema - Model for Online Conversion 10120`.

모델에 대한 채점 데이터를 유지하는 데이터 집합의 이름은 `AMM AI Aggregrate Scores - <id>`(예: `AMM AI Aggregrate Scores - 10120`)과 같이 지정됩니다.

스키마에는 점수에 대한 세부 정보가 포함된 오브젝트가 있는 필드 그룹이 포함됩니다. 객체는 다음 필드로 구성됩니다.

| 필드 이름 | 유형 | 정의 |
|---|---|---|
| `campaignGroup` | 문자열 | 캠페인 그룹 이름. |
| `campaignName` | 문자열 | 캠페인 이름. |
| `contribution` | Double | 지정된 터치포인트에 대한 이 전환에 기인한 기여입니다. |
| `conversionEndDate` | 날짜 | 전환 창의 종료 날짜. |
| `conversionName` | 문자열 | 전환 정의 설정 단계 중에 생성된 전환의 이름입니다. |
| `conversionStartDate` | 날짜 | 전환 창의 시작일. |
| `geo` | 문자열 | 전환이 발생한 지리적 위치. |
| `mediaChannel` | 문자열 | 터치포인트 설정 단계 중에 사용된 채널의 이름입니다. |
| `mediaSubChannel` | 문자열 | 하위 채널 이름. |
| `revenue` | Double | 지정된 접점에 대한 이 전환으로 인한 매출입니다. |
| `scoreCreatedTime` | DateTime | 해당 스코어 레코드가 생성될 때의 타임스탬프. |
| `touchpointEndDate` | 날짜 | 접점 창의 종료 날짜입니다. |
| `touchpointName` | 문자열 | 접점 정의 설정 단계 중에 생성된 접점 이름입니다. 현재 터치포인트는 미디어 채널에 정의되어 있습니다. |
| `touchpointStartDate` | 날짜 | 접점 창의 시작 날짜입니다. |


## 이벤트 점수 데이터 스키마

채점 데이터에 대한 스키마의 이름은 `Attribution AI Scores - <name of model> <id> - Schema`과(와) 같이 지정됩니다. 예: `Attribution AI Scores - Model for Online Conversion 10120 - Schema`.

모델에 대한 채점 데이터를 유지하는 데이터 집합의 이름은 `Attribution AI Scores - <name of model> <id>`(예: `Attribution AI Scores - Model for Online Conversion 10120 `)과 같이 지정됩니다.

스키마에는 코어에 대한 세부 사항이 포함된 오브젝트가 포함된 필드 그룹이 포함됩니다. 개체 이름은 `attibution_AI_scores__<name of model> id`과(와) 같이 지정됩니다.

필드 그룹에는 다음 필드가 포함되어 있습니다.

| 필드 이름 | 유형 | 설명 |
|---|---|---|
| `conversion` | 오브젝트 | 전환 메타데이터 열입니다. |
|     `passThrough` | 오브젝트 |  |
|         `eventType` | 문자열 | |
|         `channel_typeAtSource` | 문자열 | |
|      `dataSource` | 문자열 | 데이터 소스에 대한 전역 고유 식별자. <br> **예:** `Adobe Analytics` |
|      `eventSource` | 문자열 | 실제 이벤트가 발생한 소스. <br> **예:** `Adobe.com` |
|      `eventType` | 문자열 | 해당 시계열 레코드에 대한 기본 이벤트 유형. <br> **예:** `Order` |
|      `geo` | 문자열 | 전환이 전달된 지리적 위치 `placeContext.geo.countryCode`입니다. <br> **예:** `US` |
|      `path` | 문자열 | |
|      `priceTotal` | Double | 전환 <br>을(를) 통해 얻은 매출 **예:** `99.9` |
|      `product` | 문자열 | 제품 자체의 XDM 식별자. <br> **예:** `RX 1080 ti` |
|      `productType` | 문자열 | 이 제품 보기에 대해 사용자에게 표시되는 제품의 표시 이름입니다. <br> **예:** `Gpus` |
|      `quantity` | 정수 | 전환 중 구매한 수량입니다. <br> **예:** `1` |
|      `receivedTimeStamp` | DateTime | 전환의 타임스탬프를 수신했습니다. <br> **예:** `2020-06-09T00:01:51.000Z` |
|      `skuId` | 문자열 | 공급업체가 정의한 제품에 대한 고유 식별자인 SKU(Stock Keeping Unit). <br> **예:** `MJ-03-XS-Black` |
|      `timestamp` | DateTime | 변환의 타임스탬프입니다. <br> **예:** `2020-06-09T00:01:51.000Z` |
|      `totalDaysToConversion` | 정수 |  |
|      `totalTouchpointCount` | 정수 | |
| `customerProfile` | 오브젝트 | 모델 구축에 사용된 사용자의 ID 세부 정보. |
|      `identity` | 오브젝트 | |
|           `id` | 문자열 | |
|           `namespace` | 문자열 | `id` 및 `namespace` 등 모델을 만드는 데 사용되는 사용자의 세부 정보를 포함합니다. |
| `touchpointsDetail` | 개체[] | 전환으로 이어지는 접점 세부 정보 목록으로서, 접점 발생 또는 타임스탬프별로 순서가 지정됩니다. |
|      `scores` | 오브젝트 | 이 전환에 대한 터치포인트 기여도를 점수로 표시합니다. |
|           `algorithmicInfluenced` | Double | 영향을 받는 점수는 각 마케팅 접점이 담당하는 전환의 비율입니다. |
|           `algorithmicSourced` | Double | 증분 점수는 마케팅 접점에 의해 직접 발생한 한계 영향의 양입니다. |
|           `decayUnits` | Double | 전환에 더 가까운 접점이 전환에서 시간상 더 먼 접점보다 더 많은 크레딧을 받는 규칙 기반 속성 점수. |
|           `firstTouch` | Double | 전환 경로의 초기 접점에 모든 크레딧을 할당하는 규칙 기반 속성 점수입니다. |
|           `lastTouch` | Double | 전환에 가장 가까운 접점에 모든 크레딧을 할당하는 규칙 기반 속성 점수. |
|           `linear` | Double | 전환 경로의 각 접점에 동일한 크레딧을 할당하는 규칙 기반 속성 점수. |
|           `uShape` | Double | 첫 번째 접점에 크레딧의 40%를 할당하고 마지막 접점에 크레딧의 40%를 할당하는 규칙 기반 속성 점수입니다. 나머지 20%는 다른 접점에서 똑같이 나누어집니다. |
|      `touchPoint` | 오브젝트 | 접점 메타데이터. |
|           `passThrough` | 오브젝트 | |
|                `eventType` | 문자열 | |
|           `campaignGroup` | 문자열 |  |
|           `campaignName` | 문자열 | |
|           `campaignTag` | 문자열 | |
|           `eventId` | 문자열 | |
|           `geo` | 문자열 | |
|           `mediaAction` | 문자열 | |
|           `mediaChannel` | 문자열 | |
|           `receivedTimeStamp` | DateTime | |
|           `timestamp` | DateTime | |
|      `isFirstInThePosition` | 정수 | |
|      `lag` | 정수 | |
|      `position` | 문자열 | |
|      `touchpointCountToConversion` | 정수 | |
|      `touchpointName` | 문자열 | 설정 중에 구성된 터치포인트의 이름입니다. <br> **예:** `PAID_SEARCH_CLICK` |
| `conversionName` | 문자열 | 설정 중에 구성된 전환의 이름입니다. <br> **예:** `Order`, `Lead`, `Visit` |
| `scoreCreatedTime` | DateTime | |
| `segmentation` | 문자열 | 모델이 만들어지는 지역 세분화와 같은 전환 세그먼트. 세그먼트가 없으면 `segmentation`은(는) `conversionName`과(와) 같습니다. <br> **예:** `ORDER_US` |





자세한 내용은 [스키마](../ingest-data/schemas.md)를 참조하십시오.
