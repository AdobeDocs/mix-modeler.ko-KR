---
title: 채점 데이터
description: Mix Modeler에서 모델의 채점 데이터가 어떻게 지속되는지 알아봅니다.
feature: Models
source-git-commit: 3596b83937b3f61ac453940f3a666d8aaf713679
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 7%

---


# 채점 데이터

모델에 대한 채점을 수행하는 과정에서 채점 데이터는 Experience Platform의 데이터 세트 내에서 유지됩니다. 이 데이터 세트는 Mix Modeler 인스턴스의 각 모델에 대해 만들어진 스키마를 따릅니다.

채점 데이터에 대한 스키마의 이름은 다음과 같습니다 `AMM AI Schema - <name of model> <id>`. For example: `AMM AI Schema - Model for Online Conversion 10120`.

모델에 대한 채점 데이터를 유지하는 데이터 세트의 이름은 다음과 같습니다 `AMM AI Aggregrate Scores - <id>`, 예 `AMM AI Aggregrate Scores - 10120`.


## 스키마

스키마에는 점수에 대한 세부 정보가 포함된 오브젝트가 있는 필드 그룹이 포함됩니다. 객체는 다음 필드로 구성됩니다.

| 필드 이름 | 유형 | 정의 |
|---|---|---|
| **campaignGroup** | 문자열 | 캠페인 그룹 이름. |
| **campaignName** | 문자열 | 캠페인 이름. |
| **기여도** | 이중 | 지정된 터치포인트에 대한 이 전환에 기인한 기여입니다. |
| **전환 종료 날짜** | 날짜 | 전환 창의 종료 날짜. |
| **conversionName** | 문자열 | 전환 정의 설정 단계 중에 생성된 전환의 이름입니다. |
| **conversionStartDate** | 날짜 | 전환 창의 시작일. |
| **지역** | 문자열 | 전환이 발생한 지리적 위치. |
| **mediaChannel** | 문자열 | 터치포인트 설정 단계 중에 사용된 채널의 이름입니다. |
| **mediaSubChannel** | 문자열 | 하위 채널 이름. |
| **매출** | 이중 | 지정된 접점에 대한 이 전환으로 인한 매출입니다. |
| **scoreCreatedTime** | DateTime | 이 스코어 레코드를 만드는 시간입니다. |
| **터치포인트 종료 날짜** | 날짜 | 접점 창의 종료 날짜입니다. |
| **터치포인트 이름** | 문자열 | 접점 정의 설정 단계 중에 생성된 접점 이름입니다. 현재 터치포인트는 미디어 채널에 정의되어 있습니다. |
| **touchpointStartDate** | 날짜 | 접점 창의 시작 날짜입니다. |

