---
title: 현재 Mix Modeler 릴리스 정보 보기
description: 최신 Mix Modeler 릴리스 정보
feature-set: Experience Cloud
feature: Release Notes
exl-id: 38a47672-2af2-437c-b769-4d5febb941f5
source-git-commit: 498f50e4d1568e58d0ac2833022822340a5f6337
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 4%

---

# 최신 Mix Modeler 릴리스 정보

**마지막 업데이트**: 2025년 5월 14일.

이 릴리스 노트는 Mix Modeler의 최신 릴리스를 다룹니다. Mix Modeler 릴리스는 연속 게재 모델에서 작동하므로 대략적인 월별 릴리스 케이던스를 사용할 수 있습니다. 따라서 이 릴리스 정보는 업데이트되므로 정기적으로 확인하십시오.


## 2025년 5월 - 6월

| 기능 | 설명 | [롤아웃 시작](#release-strategy) | [일반 가용성](#release-strategy) |
|---|---|---|---|
| **목표 기반 계획** | 플랜 [만들기](/help/plans/build.md) 또는 [편집](/help/plans/insights.md#edit-plan)할 때 예산 옆에서 목표(대상)를 정의할 수 있습니다. 타겟 지표의 예로는 매출, 전환, CPA 또는 ROI가 있습니다. | 2025년 6월 18일 목요일 | 2025년 7월 8일 수요일 |
| **지출 패턴 구성** | 이제 플랜을 작성할 때 각 예산 날짜 범위에 대한 지출 패턴을 정의할 때 [과거 참조](/help/plans/build.md) 데이터(예: 과거 마케팅 지출 데이터 및 통찰력)를 사용할 수 있는 옵션이 제공됩니다. | 2025년 5월 14일 | 2025년 5월 14일 |
| **고급 계획 구성** | 플랜에 대해 전환당 평균 매출액 및 채널 비용과 같은 [고급 구성](/help/plans/build.md)을 정의할 수 있습니다. | 2025년 5월 14일 | 2025년 5월 14일 |

## 2025년 3월 - 4월

| 기능 | 설명 | [롤아웃 시작](#release-strategy) | [일반 가용성](#release-strategy) |
|---|---|---|---|
| **모델 드리프트 감지** | 모델을 열면 모델 드리프트가 감지될 때 [모델을 다시 교육하라는 메시지가 표시됩니다](/help/models/insights.md#model-drift). | 2025년 4월 3일 | 2022년 5월 7일 |
| **계획 인사이트에서 한계 채널 반환** | [한계 채널 반환](/help/plans/insights.md#marginal-channel-return) 시각화가 계획 인사이트에 추가되어 모든 또는 선택한 채널에 대한 한계 브레이크 이벤트 및 계획 반환을 표시합니다. | 2025년 4월 3일 | 2025년 4월 24일 |


## 2025년 1월 - 2월

| 기능 | 설명 | [롤아웃 시작](#release-strategy) | [일반 가용성](#release-strategy) |
|---|---|---|---|
| **중첩 조건** | [모델의 구성](/help/models/build.md#configure)의 일부로 적격한 데이터 모집단을 정의할 때 AND 및 OR을 사용하여 중첩 조건을 만들 수 있습니다. | 2025년 1월 15일 | 2025년 2월 18일 |
| **보고서 보기** | 데이터 조화의 일부로 정의한 [전환](/help/harmonize-data/conversions.md#view-report) 또는 [마케팅 접점](/help/harmonize-data/marketing-touchpoints.md#view-report)에 대한 보고서를 볼 수 있습니다. | 2025년 1월 15일 | 2025년 2월 18일 |
| **확인 삭제** | [플랜](/help/plans/overview.md#delete-plans) 또는 [모델](/help/models/overview.md#delete-models)의 삭제를 확인하는 메시지가 표시됩니다. | 2025년 1월 15일 | 2025년 2월 18일 |
| **UI 개선 요소** | 모델 인사이트에 표시할 [요소](/help/models/insights.md#factors-beta)를 선택할 수 있습니다. | 2025년 1월 15일 | 2025년 2월 18일 |
| **오류 처리** | 사용자 친화적인 오류 메시지 및 데이터 조화 및 계획의 오류 시나리오에 대한 사용자 경험 개선. | 2025년 2월 18일 | 2025년 2월 18일 |
| **모델 상태** | 모델 라이프사이클에서 [모델 상태](/help/models/overview.md#manage-models)를 재정의합니다. | 2025년 2월 18일 | 2025년 2월 18일 |


## 릴리스 전략

[!UICONTROL Mixx Modeler]은(는) 기능 플래그(&quot;전환&quot;이라고도 함)를 사용하여 새로운 기능의 가시성을 제어하므로 전체 릴리스 전에 통제된 크기 테스트를 수행할 수 있습니다. 이 릴리스 전략에는 다음 단계가 포함됩니다.

* **제한된 테스트**: 단계적인 릴리스는 내부 Adobe 사용자에 의한 테스트부터 시작됩니다. 이 기능은 고객의 요구 사항과 기대에 부응할 수 있도록 소규모 고객 고객 그룹이 사용할 수 있습니다.

* **롤아웃 시작**: 단계적인 릴리스 롤아웃은 제한된 테스트 단계에서 시작됩니다. 그런 다음 몇 개월 동안 고객에게 릴리스의 가용성이 0%에서 100%로 확장됩니다. 단계적 롤아웃은 Experience Cloud 조직 수준에서 발생하므로 조직의 모든 권한 있는 사용자는 동일한 경험을 받습니다.
