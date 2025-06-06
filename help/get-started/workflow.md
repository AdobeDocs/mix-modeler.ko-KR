---
title: Mix Modeler 워크플로
description: Mix Modeler의 일반적인 워크플로를 이해합니다.
feature: Ingest Data, Plans, Harmonized Data, Models
exl-id: 200ff846-5d78-4b25-a425-bfd558b88c88
source-git-commit: bdb5992ba1e6a4e5aa546b6ffb8e9673ed69be22
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# Mix Modeler 워크플로

Mix Modeler의 사용자 워크플로우에 대한 소개는 이 비디오 를 참조하십시오.

>[!VIDEO](https://video.tv.adobe.com/v/3440210/?learn=on&captions=kor)


Mix Modeler의 일반적인 워크플로우는 다음 활동으로 구성됩니다.

![대체 텍스트](/help/assets/ApplicationWorkflow.svg)

|  | 활동 | 설명 |
|---|---|---|
| ![데이터](/help/assets/icons/Data.svg){width="100"} | [**데이터 수집**](../ingest-data/overview.md) | Experience Platform의 이벤트 데이터(예: Adobe Analytics, Web SDK, 기타 소스), 마케팅 채널의 집계 데이터(예: TV, 벽으로 둘러싸인 정원, 이메일, 소유 및 운영되는 활동), 고객의 외부 요인 데이터(예: 구독 서비스의 가격 변경) 및 내부 요인 데이터(예: 휴일 플랜)를 수집합니다. |
| ![DataCheck](/help/assets/icons/DataCheck.svg){width="100"} | [**데이터 통합**](../harmonize-data/overview.md) | 매핑 규칙 및 충돌 해결 규칙을 구성하여 Mix Modeler에서 캠페인 성과를 측정하고 계획하는 데 필요한 다양한 마케팅 데이터 세트를 병합합니다. |
| ![FileConfig](/help/assets/icons/FileGear.svg){width="100"} | [**모델 빌드**](../models/overview.md) | 마케팅 접점(예: 채널), 전환 정의 및 내부 및 외부 요인이 있는 모델 인스턴스를 빌드합니다. |
| ![파일 데이터](/help/assets/icons/FileData.svg){width="100"} | [**교육 및 점수 모델**](../models/overview.md) | 머신 러닝 교육 및 채점을 사용하여 집계 및 이벤트 수준 점수를 만드십시오. |
| ![파일 차트](/help/assets/icons/FileChart.svg){width="100"} | [**계획 작성**](../plans/overview.md) | 계획을 만들고 빌드합니다. Mix Modeler 모델의 결과를 사용하여 비즈니스 목표를 달성하기 위한 마케팅 자금의 최상의 할당을 결정합니다. |
| ![대시보드](/help/assets/icons/Dashboard.svg){width="100"} | [**개요 대시보드**](../dashboard/overview.md) | 구성 가능한 다양한 시각화를 사용하여 조정된 데이터, 모델 및 계획에 대한 통찰력을 얻으십시오. |

{style="table-layout:auto"}

입력 데이터가 Mix Modeler으로 유입될 수 있는 방법과 Mix Modeler이 자체 인터페이스뿐만 아니라 Customer Journey Analytics과 같은 다른 솔루션에 대한 출력 데이터를 생성하는 방법에 대한 개요가 아래에 나와 있습니다.

![Mix Modeler 입력 출력 데이터 흐름](../assets/mm-input-output.png)
<!---
The detailed data-oriented flowchart below illustrates how:

* harmonized data is based on:

  * experience event data (originating from Analytics source connector, collected through Experience Platform SDKs and APIs, ingested through source connectors, or using streaming ingestion),
  * aggregate or summary data from walled gardens (like Facebook, YouTube), traffic sources, or offline advertising data, and 
  * definitions of harmonized fields and dataset rules.

* a model is based on:

  * the conversion and marketing touchpoint definitions resulting from the harmonized data and 
  * non-marketing aggregate or summary data containing internal or external factors.

* mult-touch attribution event scores can potentially be fed back into Experience Platform data lake for use in subsequent model configuration, training and scoring.

![Comprehensive workflow](/help/assets/comprehensive-workflow.svg)

-->
