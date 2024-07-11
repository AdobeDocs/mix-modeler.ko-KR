---
title: Mix Modeler 워크플로
description: Mix Modeler의 일반적인 워크플로를 이해합니다.
feature: Ingest Data, Plans, Harmonized Data, Models
exl-id: 200ff846-5d78-4b25-a425-bfd558b88c88
source-git-commit: 9085363e951a4e306c64ad28f56e2c15b4a6029a
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# Mix Modeler 워크플로

Mix Modeler의 사용자 워크플로에 대한 소개는 이 비디오 를 참조하십시오.

>[!VIDEO](https://video.tv.adobe.com/v/3424854/?learn=on)


Mix Modeler의 일반적인 워크플로우는 다음 활동으로 구성됩니다.

![대체 텍스트](/help/assets//ApplicationWorkflow.svg)

|  | 활동 | 설명 |
|---|---|---|
| ![데이터](/help/assets//icons/Data.svg){width="100"} | [**데이터 수집**](../ingest-data/overview.md) | Experience Platform(예: Adobe Analytics, Web SDK, 기타 소스)의 이벤트 데이터, 마케팅 채널의 집계 데이터(예: TV, 담벼락 정원, 이메일, 소유 및 운영 활동), 고객의 외부 요인 데이터(예: 구독 서비스의 가격 변경) 및 내부 요인 데이터(예: 휴일 플랜)를 수집합니다. |
| ![DataCheck](/help/assets//icons/DataCheck.svg){width="100"} | [**데이터 조화**](../harmonize-data/overview.md) | 매핑 규칙 및 충돌 해결 규칙을 구성하여 Mix Modeler에서 캠페인 성과를 측정하고 계획하는 데 필요한 다양한 마케팅 데이터 세트를 병합합니다. |
| ![파일 구성](/help/assets//icons/FileGear.svg){width="100"} | [**모델 구성**](../models/create.md) | 마케팅 접점(예: 채널), 전환 정의 및 내부 및 외부 요인으로 모델 인스턴스를 구성합니다. |
| ![파일 데이터](/help/assets//icons/FileData.svg){width="100"} | [**교육 및 점수 모델**](../models/overview.md) | 머신 러닝 교육 및 채점을 사용하여 집계 및 이벤트 수준 점수를 만드십시오. |
| ![파일 차트](/help/assets//icons/FileChart.svg){width="100"} | [**계획 만들기**](../plans/overview.md) | Mix Modeler 모델의 결과를 사용하여 비즈니스 목표를 달성하기 위한 마케팅 자금의 최상의 할당을 결정합니다. |
| ![대시보드](/help/assets//icons/Dashboard.svg){width="100"} | [**개요 대시보드**](../dashboard/overview.md) | 다양한 구성 가능한 위젯을 사용하여 결합된 데이터, 모델 및 플랜에 대한 통찰력을 얻으십시오. |

{style="table-layout:auto"}

아래의 자세한 데이터 기반 순서도는 다음 방법을 보여 줍니다.

* harmonized data는 다음을 기반으로 합니다.

   * 경험 이벤트 데이터(Analytics 소스 커넥터에서 시작되고, Experience Platform SDK 및 API를 통해 수집되고, 소스 커넥터를 통해 수집되거나, 스트리밍 수집 사용),
   * 벽으로 둘러싸인 정원(예: Facebook, YouTube), 트래픽 소스 또는 오프라인 광고 데이터의 집계 또는 요약 데이터
   * harmonized fields 및 dataset 규칙의 정의.

* 모델은 다음을 기반으로 합니다.

   * 통합 데이터 및 로 인한 전환 및 마케팅 접점 정의
   * 내부 또는 외부 요소가 포함된 비마케팅 집계 또는 요약 데이터입니다.

* 다중 터치 속성 이벤트 점수는 후속 모델 구성, 교육 및 점수에 사용하기 위해 Experience Platform 데이터 레이크로 피드백될 수 있습니다.

![포괄적인 워크플로우](/help/assets//comprehensive-workflow.svg)
