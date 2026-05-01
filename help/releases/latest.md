---
title: 현재 Mix Modeler 릴리스 정보 보기
description: 최신 Mix Modeler 릴리스 정보
feature-set: Experience Cloud
feature: Release Notes
exl-id: 38a47672-2af2-437c-b769-4d5febb941f5
TQID: https://experienceleague.adobe.com/8o2hpkneIUMbBNEZfw9TsQLaGuPOxqF-XA2TV9cJnqc
product_v2:
  - id: b88c80e3-31df-4609-989d-d4dac0e6d973
feature_v2:
  - id: ca6bcd6f-f5ca-4e5f-a5ae-7dce7177bde9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: bcc5edb5-84c3-4940-9f84-ed88b6c16274
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
autotag-review: '2026-05-01T09:06:55.437Z'
source-git-commit: 5579087b9381c4d8e909ed5fe3099fd42d5c6799
workflow-type: tm+mt
source-wordcount: 435
ht-degree: 5%

---

# 최신 Mix Modeler 릴리스 정보

**마지막 업데이트**: 2026년 2월 26일.

이 릴리스 노트는 Mix Modeler의 최신 릴리스를 다룹니다. Mix Modeler 릴리스는 연속 게재 모델에서 작동하므로 대략적인 월별 릴리스 케이던스를 사용할 수 있습니다. 따라서 이 릴리스 정보는 업데이트되므로 정기적으로 확인하십시오.

## 2026년 3월

| 기능 | 설명 | [롤아웃 시작](#release-strategy) | [일반 가용성](#release-strategy) |
|---|---|---|---|
| **채널 adstock** | [채널 adstock](/help/models/build.md#channel-adstock)을 통해 도메인 전문 지식, 실험 결과 또는 이전 채널 분석을 모델 고급 구성에 직접 통합할 수 있습니다. 모델의 채널 분석 내에서 [채널 adstock 인사이트](/help/models/insights.md#channel-adstock)를 표시합니다. | 2026년 3월 30일 | 2026년 3월 30일 |

## 2026년 2월

| 기능 | 설명 | [롤아웃 시작](#release-strategy) | [일반 가용성](#release-strategy) |
|---|---|---|---|
| **통합 요소 워크플로** | 이제 계수가 [결합된 계수 워크플로](/help/harmonize-data/overview.md#factors)의 일부로 관리됩니다. 이를 통해 [요소 데이터를 정의](/help/ingest-data/schemas.md#factor-standard-fields-field-group)하는 방법, [데이터 집합 규칙의 일부로 내부 및 외부 요소를 관리](/help/harmonize-data/dataset-rules.md#factor-datasets)하는 방법, [모델](/help/models/build.md#configure)에서 요소 데이터를 사용하는 방법을 간소화합니다. | 2026년 2월 25일 | 2026년 2월 25일 |
| **[!UICONTROL Granular incrementality reporting]** | 별도의 모델을 만들지 않고도 [세부 인사이트 보고 필드](/help/models/build.md#granular-insights-reporting-fields)를 사용하여 모델 보고에서 드릴다운할 수 있도록 통합 필드를 정의합니다. | 2026년 2월 18일 | 2026년 2월 18일 |

## 2026년 1월

| 기능 | 설명 | [롤아웃 시작](#release-strategy) | [일반 가용성](#release-strategy) |
|---|---|---|---|
| **[!UICONTROL Dataset rules]** | [데이터 집합 규칙 테이블을 업데이트했습니다](/help/harmonize-data/dataset-rules.md). 하나 이상의 데이터 세트 규칙을 검색하고 테이블에서 직접 데이터 세트 규칙을 보거나, 편집하거나, 삭제할 수 있습니다. | 2026년 1월 13일 | 2026년 1월 13일 |
| **[!UICONTROL Current spend]** | 모델 인사이트의 [한계 응답 곡선 시각화](/help/models/insights.md#marginal-response-curves)에 현재 소비점을 추가하십시오. | 2026년 1월 13일 | 2026년 1월 13일 |
| **[!UICONTROL Sort and resize columns]** | [모델](/help/models/overview.md) 및 [계획](/help/plans/overview.md) 표에 열의 정렬 및 크기 조정을 추가했습니다. | 2026년 1월 13일 | 2026년 1월 13일 |
| **수정 사항** | 다음 티켓에 대한 수정 사항: <ul><li>AMM-3328: 요인에 대한 새 연산자에 대해 필드 입력이 비활성화됨</li><li>AMM-3359: 날짜 선택기 및 콤보 상자 잠금.</li><li>AMM-3441: 계획을 복제해도 일자 범위 및 예산이 자동으로 채워지지 않습니다.</li></ul> | 2026년 1월 13일 | 2026년 1월 13일 |


## 릴리스 전략

[!UICONTROL Mix Modeler]은(는) 기능 플래그(&quot;전환&quot;이라고도 함)를 사용하여 새로운 기능의 가시성을 제어하므로 전체 릴리스 전에 통제된 크기 테스트를 수행할 수 있습니다. 이 릴리스 전략에는 다음 단계가 포함됩니다.

* **제한된 테스트**: 단계적인 릴리스는 내부 Adobe 사용자에 의한 테스트부터 시작됩니다. 이 기능은 고객의 요구 사항과 기대에 부응할 수 있도록 소규모 고객 고객 그룹이 사용할 수 있습니다.

* **롤아웃 시작**: 단계적인 릴리스 롤아웃은 제한된 테스트 단계에서 시작됩니다. 그런 다음 몇 개월 동안 고객에게 릴리스의 가용성이 0%에서 100%로 확장됩니다. 단계적 롤아웃은 Experience Cloud 조직 수준에서 발생하므로 조직의 모든 권한 있는 사용자는 동일한 경험을 받습니다.

