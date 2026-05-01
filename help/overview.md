---
title: Mix Modeler 안내서
description: Mix Modeler를 사용하여 모든 채널에서 캠페인을 측정하고 계획 수립을 전체적으로 최적화하는 방법에 대해 알아봅니다.
short-description: Mix Modeler를 사용하여 모든 채널에서 캠페인을 측정하고 계획 수립을 전체적으로 최적화하는 방법에 대해 알아봅니다.
feature: Harmonized Data, Models, Plans
exl-id: 3427c338-f2a0-416b-bb4c-d8fef929c38a
TQID: https://experienceleague.adobe.com/XGSUhG3iwdjNowmk8AM87eCKv-JZF1DDAYzW0uktpes
autotag-review: '2026-05-01T09:02:01.855Z'
product_v2:
  - id: b88c80e3-31df-4609-989d-d4dac0e6d973
feature_v2:
  - id: f40f1683-8300-4054-aab8-77da06ad63ff
  - id: a567f0f7-0057-4079-8ded-5b24cc25af15
  - id: fe1c9ae8-a908-4ae1-a0b6-fcf35177b134
  - id: a234aebd-3855-4376-a64d-29b38411e0c5
  - id: d822825b-9821-40d5-9b0d-42a9e3f317c5
subfeature_v2:
  - id: a9505d76-24a1-4ffe-bd01-6ac32d5af453
  - id: ba4fd72c-282e-4fb6-abc1-08e6fb87b2ad
  - id: bc2f5225-03d4-4bc8-89ec-99d78c30e6dd
  - id: c89e26b6-808d-4500-8b01-450a63466999
  - id: cb40363e-1205-4921-971c-9ee6bdb18329
  - id: b2d4aeb9-eabe-49f6-8edb-bb2862d5980b
  - id: b4655f7e-1a6e-4fa3-a7c5-3c34d4786e49
  - id: d4b8ba18-64c1-4413-be54-74405ec7f558
  - id: d7b067e6-4f39-41e9-a081-7650346a84cd
  - id: b2520ae7-8f6c-4952-935e-aacc2c10256f
  - id: e6c284e0-b6e6-4f82-bf96-e96bb5157b90
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 5579087b9381c4d8e909ed5fe3099fd42d5c6799
workflow-type: tm+mt
source-wordcount: 236
ht-degree: 14%

---

# Adobe Mix Modeler 안내서

이 기술 설명서는 Adobe **Mix Modeler**&#x200B;에 대한 자가 진단 지원을 제공합니다. Mix Modeler은 캠페인을 측정하고 유료, 수익 및 소유 등 모든 채널에서 전체적으로 계획을 최적화하는 Adobe Experience Cloud 애플리케이션입니다. Mix Modeler은 Adobe Experience Platform의 맨 위에 구축되었으며 Adobe Sensei에서 지원합니다.

## 기본 사항부터 시작

<table style="table-layout:fixed">
  <tr style="border: 0;">
    <td>
    <a href="/help/get-started/about.md"><img src="assets/whatis-mm.png"></a>
    <div><strong>빠른 시작</strong><br/>Mix Modeler의 워크플로에 대한 및 insight의 개요를 살펴보십시오.</div>
    </td>
    <td>
    <a href="/help/ingest-data/overview.md"><img src="assets/data-ingestion-mm.png"></a>
    <div><strong>데이터 수집</strong><br/>이벤트 및 집계 또는 요약 데이터를 Mix Modeler으로 수집하는 방법에 대해 알아봅니다.</div>
    </td>
    <td>
    <a href="/help/harmonize-data/overview.md"><img src="assets/plan-mm.png"/></a>
    <div><strong>데이터 통합</strong><br/>집계 및 이벤트 데이터를 일관된 데이터 보기에 통합하는 방법을 알아봅니다. 
    </div>
    </td>
    <td>
    <a href="/help/models/overview.md"><img src="assets/models-mm.png"></a>
    <div><strong>모델 및 계획</strong><br/>모델을 교육하고 평가하여 마케팅 계획에 대한 인사이트를 사용합니다.</div>
    </td>
  </tr>
  <tr style="border: 0;">
    <td align="center"><a href="/help/get-started/about.md"><img src="assets/learn-more-button.svg"></a></td>
    <td align="center"><a href="/help/ingest-data/overview.md"><img src="assets/learn-more-button.svg"></a></td>
    <td align="center"><a href="/help/harmonize-data/overview.md"><img src="assets/learn-more-button.svg"></a></td>
    <td align="center"><a href="/help/models/overview.md"><img src="assets/learn-more-button.svg"></a></td>
    </tr>
</table>


## 설명서 살펴보기

<table style="table-layout:fixed">
  <tr style="border: 0;">
    <td>
      <img src="assets/Data.svg" width="35px"><br/>
      <strong>데이터 수집</strong><br/><a href="/help/ingest-data/overview.md">개요</a> - <a href="/help/ingest-data/schemas.md">스키마</a> - <a href="/help/ingest-data/datasets.md">데이터 세트</a> 
    </td>
    <td>
      <img src="assets/DataCheck.svg" width="35px"><br/>
      <strong>데이터 통합</strong><br/><a href="/help/harmonize-data/overview.md">개요</a> - <a href="/help/harmonize-data/fields.md">필드</a> - <a href="/help/harmonize-data/dataset-rules.md">데이터 세트 규칙</a> - <a href="/help/harmonize-data/marketing-touchpoints.md">마케팅 접점</a> - <a href="/help/harmonize-data/conversions.md">전환</a> - <a href="/help/harmonize-data/usage-report.md">사용 보고서</a>  
    </td>
    <td>
      <img src="assets/FileGear.svg" width="35px"><br/>
      <strong>모델</strong><br/><a href="/help/models/overview.md">개요</a> - <a href="/help/models/build.md">모델 구축</a> - <a href="/help/models/insights.md">모델 인사이트</a> - <a href="/help/models/scoring-data.md">채점 데이터 사용</a>
    </td>
  </tr>
  <tr style="border: 0;">
    <td>
      <img src="assets/FileChart.svg" width="35px"><br/>
      <strong>계획</strong><br/><a href="/help/plans/overview.md">계획</a> - <a href="/help/plans/build.md">계획 작성</a> - <a href="/help/plans/compare.md">계획 비교</a> - <a href="/help/plans/build.md">계획 통찰력</a>
    </td>
    <td>
      <img src="assets/Dashboard.svg" width="35px"><br/>
      <strong>개요</strong><br/><a href="/help/dashboard/overview.md">스키마</a> - <a href="/help/dashboard/harmonized-data.md">통합 데이터</a> - <a href="/help/dashboard/plans.md">계획</a>
    </td>
        <td>
      <img src="assets/Learn.svg" width="35px"><br/>
      <strong>튜토리얼</strong><br/><a href="https://experienceleague.adobe.com/docs/mix-modeler-learn/tutorials/overview.html?lang=en">개요</a> - <a href="https://experienceleague.adobe.com/docs/mix-modeler-learn/tutorials/intro/use-cases.html?lang=en">사용 사례</a> - <a href="https://experienceleague.adobe.com/docs/mix-modeler-learn/tutorials/intro/user-workflow.html?lang=en">사용자 워크플로우</a> - <a href="https://experienceleague.adobe.com/docs/mix-modeler-learn/tutorials/intro/user-interface-tour.html?lang=en">사용자 인터페이스 둘러보기</a>
    </td>
  </tr>
</table>

