---
title: 데이터 조화
description: Mix Modeler에서 데이터를 조화롭게 구성하는 방법에 대해 알아봅니다.
feature: Harmonized Data
exl-id: 6cb70762-e3b2-46a0-b028-1d6daf3edae5
source-git-commit: 9085363e951a4e306c64ad28f56e2c15b4a6029a
workflow-type: tm+mt
source-wordcount: '893'
ht-degree: 7%

---

# 데이터 조화

Mix Modeler의 데이터는 데이터 소스에 따라 그 성격이 다르다. 데이터는 다음과 같을 수 있습니다.

* 집계 또는 요약 데이터(예: 담으로 둘러싸인 정원 데이터 소스에서 수집되거나 빌보드 캠페인, 이벤트 또는 물리적 광고 캠페인을 실행하여 수집된(지출) 오프라인 광고 데이터)
* 이벤트 데이터(예: 자사 데이터 소스). 이 이벤트 데이터는 Adobe Analytics의 Adobe Analytics 소스 커넥터, Experience Platform 웹 또는 Mobile SDK 또는 Edge Network API를 통해 수집된 데이터 또는 소스 커넥터를 사용하여 수집된 데이터일 수 있습니다.

Mix Modeler의 조화 서비스는 집계 및 이벤트 데이터를 일관된 데이터 보기로 통합합니다. 내부 및 외부 요인 데이터와 결합된 이 데이터 보기는 Mix Modeler의 모델에 대한 소스입니다. 이 서비스는 여러 데이터 세트에서 가장 높은 세부 기간을 사용합니다. 예를 들어, 한 데이터 세트에 월간 세부 기간이 있고 나머지 데이터 세트에 주별 및 일별 세부 기간이 있는 경우, 조화 서비스는 월간 세부 기간을 사용하여 데이터 보기를 만듭니다.

## 조정된 데이터의 예

Mix Modeler에 사용할 수 있는 데이터 세트가 다음과 같다고 가정합니다.

**데이터 집합 1**

집계 데이터의 세부기간을 일별로 설정하여 YouTube의 마케팅 노력 데이터 세트를 포함합니다.

| 날짜 | 날짜 유형 | 채널 | Campaign | 브랜드 | 지역 | 클릭수 | 지출 |
|---|:--:|---|---|---|---|---:|---:|
| 12-31-2021 | 일 | YouTube | Y_Fall_02 | 브랜드 | US | 10000 | 10 |
| 01-01-2022 | 일 | YouTube | Y_Fall_02 | 브랜드 | US | 1000 | 10 |
| 01-03-2022 | 일 | YouTube | Y_Fall_01 | Y 브랜드 | CA | 10000 | 100 |
| 01-04-2022 | 일 | YouTube | Y_Summer_01 | Null | CA | 9000 | 80 |

{style="table-layout:auto"}


**데이터 집합 2**

집계 데이터의 세부기간이 주별로 설정된 Facebook의 마케팅 활동 데이터 세트를 포함합니다.

| 날짜 | 날짜 유형 | 채널 | Campaign | 지역 | 클릭수 | 지출 |
|--- |:---:|--- |---|---|---:|---:|
| 01-01-2022 | 주 | Facebook | FB_Fall_01 | US | 8000 | 100 |
| 01-08-2022 | 주 | Facebook | FB_Fall_02 | US | 1000 | 10 |
| 01-08-2022 | 주 | Facebook | FB_Fall_01 | US | 7000 | 100 |
| 01-16-2022 | 주 | Facebook | FB_Summer_01 | CA | 10000 | 80 |

{style="table-layout:auto"}


**데이터 집합 3**

집계 데이터의 세부기간이 일별로 설정된 전환 데이터 세트입니다.

| 날짜 | 날짜 유형 | 지역 | 목표 | 매출 |
|--- |:---: |---|---|---:|
| 01-01-2022 | 일 | US | 패션 | 200 |
| 01-08-2022 | 일 | US | 패션 | 10 |
| 01-08-2022 | 일 | US | 보석 | 1100 |
| 01-16-2022 | 일 | CA | 보석 | 80 |

{style="table-layout:auto"}


**데이터 집합 4**

고객의 샘플 경험 이벤트 데이터 세트(웹 SDK 이벤트).

| 타임스탬프 | ID 네임스페이스 | ID | 채널 | 클릭수 |
|--- |--- |--- |--- |---:|
| 01-01-2022 00:01:01.000 | ECID | 64fd46ff-8c63-43b4-85a7-92b953113ba0 | CSE | 1 |
| 01-01-2022 00:01:01.000 | ECID | 64fd46ff-8c63-43b4-85a7-92b953113ba0 | CSE | 1 |
| 01-08-2022 00:01:01.000 | ECID | 2ca2a16e-caf0-4fa9-9a8b-9774b39547c4 | CSE | 1 |
| 01-08-2022 00:01:01.000 | ECID | 5ce99bfb-e44a-40d9-b8cd-c5408bda7cdc | CSE | 1 |

{style="table-layout:auto"}


세부기간을 주별로 설정하여 조화된 데이터 세트를 만들려고 합니다. 이벤트 데이터는 주 세부 기간으로 집계되고, 조정된 데이터 세트에 추가됩니다. 결과는 다음과 같습니다.

**통합 데이터 세트**

| 날짜 | 날짜 유형 | 채널 | Campaign | 브랜드 | 지역 | 목표 | 클릭수 | 지출 | 매출 |
|--- |:---:|--- |--- |--- |---|---|---:|---:|---:|
| 12-27-2021 | 주 | YouTube | Y_Fall_02 | 브랜드 | US | Null | 11000 | 110 | Null |
| 01-03-2022 | 주 | YouTube | Y_Fall_01 | Y 브랜드 | CA | Null | 10000 | 100 | Null |
| 01-03-2022 | 주 | YouTube | Y_Summer_01 | Null | CA | Null | 9000 | 80 | Null |
| 01-01-2022 | 주 | Facebook | FB_Fall_01 | Null | US | Null | 8000 | 100 | Null |
| 01-08-2022 | 주 | Facebook | FB_Fall_02 | Null | US | Null | 1000 | 10 | Null |
| 01-08-2022 | 주 | Facebook | FB_Fall_01 | Null | US | Null | 7000 | 100 | Null |
| 01-16-2022 | 주 | Facebook | FB_Summer_01 | Null | CA | Null | 10000 | 80 | Null |
| 12-27-2021 | 주 | Null | Null | Null | US | 패션 | Null | Null | 200 |
| 01-03-2022 | 주 | Null | Null | Null | US | 패션 | Null | Null | 10 |
| 01-03-2022 | 주 | Null | Null | Null | US | 보석 | Null | Null | 1100 |
| 01-10-2022 | 주 | Null | Null | Null | CA | 보석 | Null | Null | 80 |
| 01-01-2022 | 주 | CSE | Null | Null | Null | Null | 2 | Null | Null |
| 01-08-2022 | 주 | CSE | Null | Null | Null | Null | 2 | Null | Null |

{style="table-layout:auto"}


## 조화로운 데이터 설정

간소화된 [예제](#an-example-of-harmonized-data)에서와 같이 통합 데이터 집합을 만들려면 다음 단계를 수행해야 합니다.

1. 이미 사용 가능한 전역 조화 필드 외에 사용할 추가 [조화 필드](fields.md)을(를) 정의합니다.
1. 집계 또는 경험 이벤트 데이터 세트의 필드를 조화로운 필드에 매핑하려면 [데이터 세트 규칙](dataset-rules.md)을 설정하십시오.
1. 정의한 표준 및 추가 조화 필드를 사용하여 [마케팅 접점](marketing-touchpoints.md)을(를) 정의합니다.
1. 정의한 표준 및 추가 조화 필드를 사용하여 [전환](conversions.md)을(를) 정의합니다.


## 조화로운 데이터 보기

Mix Modeler 인터페이스에서 조정된 데이터를 보려면 다음을 수행하십시오.

1. 왼쪽 레일에서 ![DataSearch](/help/assets//icons/DataCheck.svg) **[!UICONTROL Harmonized datasets]**&#x200B;을(를) 선택합니다.

1. 상단 표시줄에서 **[!UICONTROL Harmonized Data]**&#x200B;을(를) 선택합니다. 정의한 필드, 데이터 세트 규칙, 마케팅 접점 및 전환을 기반으로 조정된 데이터의 요약이 표시됩니다.

   1. 결합된 데이터의 다시 캡을 기준으로 하는 기간을 다시 정의하려면 **[!UICONTROL Date range]**&#x200B;의 날짜 범위를 입력하거나 ![달력](/help/assets//icons/Calendar.svg)을 사용하여 데이터 범위를 선택하십시오.

   1. Harmonized 데이터 테이블에 표시되는 Harmonized 필드 열을 수정하려면 ![설정](/help/assets//icons/Setting.svg)을 사용하여 **[!UICONTROL Column settings]** 대화 상자를 엽니다.

      1. **[!UICONTROL AVAILABLE COLUMNS]**&#x200B;에서 하나 이상의 열을 ![SelectBox](/help/assets//icons/SelectBox.svg)을(를) 선택하고 ![V자형 화살표 오른쪽](/help/assets//icons/ChevronRight.svg)을(를) 사용하여 이러한 열을 **[!UICONTROL SELECTED COLUMNS]**&#x200B;에 추가하십시오.

      1. **[!UICONTROL SELECTED COLUMNS]**&#x200B;에서 하나 이상의 열을 ![SelectBox](/help/assets//icons/SelectBox.svg)을(를) 선택하고 ![왼쪽 V자형 화살표](/help/assets//icons/ChevronLeft.svg)를 사용하여 선택한 열을 제거하고 이 열을 다시 **[!UICONTROL AVAILABLE COLUMNS]**(으)로 되돌립니다.

      1. **[!UICONTROL DEFAULT SORT]**&#x200B;에서 열을 선택하고 **[!UICONTROL Ascending]** 또는 **[!UICONTROL Descending]** 간에 전환합니다.

      1. 표시되는 열의 순서를 변경하려면 끌어다 놓기 를 통해 **[!UICONTROL SELECTED COLUMNS]**&#x200B;의 열을 위아래로 이동할 수 있습니다.

   1. 열 설정 변경 내용을 제출하려면 **[!UICONTROL Submit]**&#x200B;을(를) 선택하십시오. 변경 내용을 취소하려면 **[!UICONTROL Close]**&#x200B;을(를) 선택하십시오.

1. 사용할 수 있는 페이지가 더 있는 경우 ![왼쪽 화살표](/help/assets//icons/ChevronLeft.svg) 또는 ![오른쪽 화살표](/help/assets//icons/ChevronRight.svg)(**[!UICONTROL Page _x _/_x_]**)를 사용하여 페이지 간에 이동합니다.
