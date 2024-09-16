---
title: 스키마
description: 데이터를 Mix Modeler에 수집하는 데 필요한 스키마를 관리하는 방법을 알아봅니다.
feature: Schemas
exl-id: 08289581-5af9-4422-b049-8c24105e2a8e
source-git-commit: 9a6c1f1c12ab29da80a1997cfd31ca07b38eaa22
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 3%

---

# 스키마

Experience Platform에서 수집하고 Mix Modeler에서 사용할 데이터를 지원하는 스키마를 관리하려면 다음을 수행하십시오.

1. Mix Modeler 인터페이스로 이동합니다.

1. **[!UICONTROL SETUP]** 아래의 ![스키마](/help/assets/icons/Schemas.svg) **[!UICONTROL Schemas]**&#x200B;을(를) 선택하십시오.

자세한 내용은 [스키마 UI 개요](https://experienceleague.adobe.com/docs/experience-platform/xdm/ui/overview.html?lang=en)를 참조하십시오.

## 집계 또는 요약 데이터

XDM 요약 지표 클래스를 Experience Platform에 수집하고 Mix Modeler에 사용할 집계 또는 요약 데이터의 기초가 되는 스키마의 기반으로 사용하는 것이 좋습니다.

XDM 요약 지표 클래스 사용:

- 담으로 둘러싸인 정원 데이터(예: Facebook 또는 YouTube 데이터)

- SPX(S&amp;P 500 주가 지수), 날씨 데이터 등의 외부 요인 데이터,

- 내부 요소 데이터(예: 가격 변경, 휴일 달력).

>[!IMPORTANT]
>
>수집된 데이터에 필요한 지표를 지원하려면 스키마 정의에 하나 이상의 숫자 필드(정수, Double, 부울 또는 기타 숫자 유형 사용)가 포함되어야 합니다.

아래 **[!DNL ExternalFactorSummarySchema]**&#x200B;에 표시된 대로 **[!DNL XDM Summary Metrics]** 기본 클래스를 사용하는 스키마는 간단할 수 있습니다.

![외부 요소 스키마](/help/assets/external-factors-schema.png)

이 간단한 스키마를 사용하여 다음과 같은 데이터를 포함하는 데이터 세트를 수집할 수 있습니다.

- 경쟁업체 인덱스 데이터

  | 타임스탬프 | date_type | 요소 | 값 |
  |---|---|---|--:|
  | 2020-11-28T00:00:00.000Z | 주 | competitor_index | 289.8 |
  | 2020-12-05T00:00:00.000Z | 주 | competitor_index | 291.2 |
  | 2020-12-12T00:00:00.000Z | 주 | competitor_index | 280.07 |
  | ... | ... | ... | ... |

- 공휴일 데이터

  | 타임스탬프 | date_type | 요소 | 값 |
  |---|---|---|--:|
  | 2020-11-28T00:00:00.000Z | 주 | all_holidays_flag | 0.0 |
  | 2020-12-05T00:00:00.000Z | 주 | all_holidays_flag | 0.0 |
  | 2020-12-12T00:00:00.000Z | 주 | all_holidays_flag | 0.0 |
  | 2020-12-19T00:00:00.000Z | 주 | all_holidays_flag | 0.0 |
  | 2020-12-26T00:00:00.000Z | 주 | all_holidays_flag | 1.0 |
  | ... | ... | ... | ... |


**[!DNL XDM Summary Metrics]**&#x200B;을(를) 기본 클래스로 사용하는 **[!DNL LumaPaidMarketingSchema]**&#x200B;에 대한 보다 포괄적인 예제는 아래를 참조하십시오. 스키마는 지표(**[!DNL AMMMetrics]**), 차원(**[!DNL AMMDimensions]**) 및 기타 고객별 정보(**[!DNL CustomerSpecific]**)에 대해 색상 주석이 있는 전용 필드 그룹을 사용합니다.

![요약 스키마](/help/assets/summary-schema.png)

프로필 수집의 비동기적 특성을 고려할 때 외부 소스에서 합계 또는 요약 데이터를 수집할 때 외부 Source 시스템 감사 세부 정보 필드 그룹을 스키마의 일부로 사용하는 것이 좋습니다. 이 필드 그룹은 외부 소스에 대한 감사 속성 집합을 정의합니다.


## 지원되는 데이터 유형

현재 Mix Modeler은 Experience Platform 데이터 유형의 하위 집합을 지원합니다. [스키마 컴포지션의 기본 사항](https://experienceleague.adobe.com/docs/experience-platform/xdm/schema/composition.html?lang=en#data-type)에 언급된 다음 기본 데이터 형식(필드)이 지원됩니다.

- 문자열
- 정수
- Double
- 부울
- 길게
- 짧음
- 바이트
- 날짜
- 날짜-시간
