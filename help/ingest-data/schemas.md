---
title: 스키마
description: Adobe 믹스 모델러로 데이터를 수집하는 데 필요한 스키마를 관리하는 방법을 알아봅니다.
feature: Datasets
source-git-commit: abbfc78e9fa774a240d000131f35d3dc257c15ea
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 1%

---


# 스키마

Adobe Experience Platform에서 수집하고 Adobe 믹스 모델러에서 사용할 데이터를 지원하여 스키마를 관리하려면 다음 작업을 수행하십시오.

1. Adobe 믹스 모델러 인터페이스로 이동합니다.

1. 선택 ![스키마](../assets/icons/Schemas.svg) **[!UICONTROL Schemas]**, 그 아래 **[!UICONTROL DATA MANAGEMENT]**.

다음을 참조하십시오. [스키마 UI 개요](https://experienceleague.adobe.com/docs/experience-platform/xdm/ui/overview.html?lang=en) 추가 정보.

## 집계 또는 요약 데이터

XDM 요약 지표 클래스를 Experience Platform에서 수집하고 Adobe 믹스 모델러에서 사용할 집계 또는 요약 데이터의 기초가 되는 스키마의 기반으로 사용하는 것이 좋습니다.

의 예는 아래를 참조하십시오. **[!DNL LumaPaidMarketingSchema]** 지표 ( )에 대한 기본 클래스 및 전용 필드 그룹 (색상으로 주석 처리)으로 XDM 요약 지표 사용&#x200B;**[!DNL AMMMetrics]**), 차원 (**[!DNL AMMDimensions]**) 및 기타 고객별 정보(**[!DNL CustomerSpecific]**).

![요약 스키마](../assets/summary-schema.png)

감사 속성 집합을 정의하려면 외부 소스 시스템 감사 세부 정보 필드 그룹을 외부 소스에서 합계 또는 요약 데이터를 수집하는 데 사용되는 스키마의 일부로 사용하는 것이 좋습니다.
