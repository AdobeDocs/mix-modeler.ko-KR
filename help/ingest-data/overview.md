---
title: 데이터 수집 개요
description: Mix Modeler에 데이터를 수집하는 방법에 대해 알아봅니다.
feature: Datasets, Event Datasets, Summary Datasets, Aggregate Datasets
exl-id: dc16a601-bbd9-467b-8a7e-c32654d4069a
source-git-commit: bb05cee1d4e2245cf665e5dcea17a30c5c0cf203
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 7%

---

# 데이터 수집 개요

Mix Modeler은 이벤트 수준 데이터, 다양한 담벼락 정원의 집계 또는 요약 마케팅 노력 데이터, 오프라인 광고, 내부 요인 또는 외부 요인과 같은 다른 소스의 집계 또는 요약 데이터를 사용하여 작동합니다.

고객은 XDM ExperienceEvent 또는 XDM 요약 지표를 기본 클래스로 사용하여 스키마를 기반으로 하는 데이터 세트로 Experience Platform에 수집되는 모든 종류의 데이터를 사용할 수 있습니다.

For example:

* Adobe Analytics 소스 커넥터를 사용하여 수집된 데이터는 Adobe Analytics 스키마의 기본값 또는 사용자 지정 버전에 맞는 데이터 세트로 변환되거나
* 웹, 모바일 또는 기타 모든 유형의 디바이스에서 고객 상호 작용을 수집하기 위해 Experience Platform Web SDK, Mobile SDK 또는 Edge Network Server API를 사용하여 수집된 데이터
* 벽으로 둘러싸인 정원(예: Facebook, YouTube), 트래픽 소스 또는 오프라인 광고 데이터의 집계 또는 요약 데이터,
* 모델 구축에 유용한 내부 또는 외부 요인이 포함된 비마케팅 집계 또는 요약 데이터입니다.

Experience Platform에서 지원하는 모든 종류의 메커니즘을 사용하여 경험 이벤트 수준, 총 마케팅 활동 데이터 및 다른 소스의 데이터를 수집할 수 있습니다. 수집 메커니즘에는 Experience Platform SDK, API, 소스 커넥터, 스트리밍 및 일괄 처리 수집이 포함됩니다. Adobe Mix Modeler에서 사용하기 위해 Experience Platform에서 데이터를 수집하는 방법에 대한 자세한 내용은 [데이터 수집 개요](https://experienceleague.adobe.com/ko/docs/experience-platform/ingestion/home)를 참조하십시오.

## 지침

Mix Modeler에서 사용할 수 있도록 Experience Platform에 데이터를 수집하려면 다음 지침을 따르십시오.

* 데이터 세트에 추가되는 증분 데이터에는 겹치지 않아야 합니다.
* 단일 소스의 모든 데이터는 세부기간이 동일해야 합니다.
* 날짜 및 세부기간은 데이터 세트로 수집된 모든 집계 데이터에 대한 기본 스키마의 필수 필드입니다
* 채널은 데이터 세트로 수집된 모든 마케팅 활동/지출 데이터에 대한 기본 스키마의 필수 필드입니다.


## 예시

아래에서는 보다 표준적인 경험 이벤트 데이터 외에 Mix Modeler에서 일반적으로 사용되는 데이터의 몇 가지 예를 살펴봅니다.

+++ 마케팅 활동 집계 데이터

| 지역 | 일자 | 날짜 유형 | 채널 | Campaign | 클릭 | 소득 | 참여 | 노출 횟수 | 열기 | 소유 | 보냄 | 지출 |
|---|:--|---|:---:|---|--:|---|--:|---|---|---|--:|--:|
| AMER | 2021-10-31 | 일 | 이메일 | | 12752 | | | | | | 1132945 | |
| AMER | 2021-10-31 | 일 | FB | | 148844 | | | | | | | 42111 |
| AMER | 2021-10-31 | 일 | YT | | | | 2314452 | | | | | 10540 |
| 일본 | 2021-10-21 | 일 | 이메일 | | 21089 | | | | | | 3283626 | |
| 일본 | 2021-10-21 | 일 | 소셜 | | | | 621 | | | | | 74512 |

{style="table-layout:auto"}

+++

+++ 전환 데이터 집계

| 지역 | 일자 | 날짜 유형 | 제품 | 판매 수량 | 매출 |
|---|:---|:---:|---|--:|--:|
| EMEA | 2021-09-13 | 일 | 크리에이터 경제 | 603 | 36537.68 |
| EMEA | 2021-09-13 | 일 | 메타버스 | 55 | 21704.37 |
| 일본 | 2022-05-30 | 일 | Pro Imaging | 487 | 64469.60 |
| 일본 | 2022-05-30 | 일 | Document Cloud | 642 | 100509.07 |

{style="table-layout:auto"}

+++

+++ 외부 요인 데이터

| 데이터 | 날짜 유형 | 요소 | 값 |
|---|:---:|:---:|:---|
| 2020년 8월 2일 | 주 | SPX | 3325.866 |
| 2020년 8월 9일 | 주 | SPX | 3364.158 |
| 2020-08-16 | 주 | SPX | 3385.858 |
| 2020년 8월 23일 | 주 | SPX | 3497.965 |

{style="table-layout:auto"}

+++

Mix Modeler의 데이터로 작업하려면 데이터 세트에 수집된 데이터와 Experience Platform의 스키마를 모델로 해야 합니다. Mix Modeler 인터페이스를 사용하면 Experience Platform 스키마 및 데이터 세트 UI에 쉽게 액세스할 수 있습니다.


## 유효성 검사

Mix Modeler에서 데이터를 제대로 사용할 수 있는지 확인하려면 다음을 수행할 수 있습니다.

* [개요](/help/overview.md)에서 시각화를 사용합니다.
* Harmonized 데이터 세트의 [Harmonized data](/help/harmonize-data/overview.md)에서 데이터를 다운로드하고 검사합니다.

데이터가 Experience Platform에서 제대로 수집되었는지 확인하기 위해 [Experience Platform 쿼리 서비스를 사용하여 SQL 쿼리를 쓰고 실행](https://experienceleague.adobe.com/ko/docs/experience-platform/query/home)할 수 있습니다.


>[!MORELIKETHIS]
>
>스키마 및 데이터 세트를 관리하는 방법에 대한 자세한 내용은 를 참조하십시오.
>
>* [스키마](schemas.md)
>* [데이터 세트](datasets.md)
