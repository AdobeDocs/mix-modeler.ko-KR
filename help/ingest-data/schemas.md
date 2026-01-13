---
title: 스키마
description: Mix Modeler으로 데이터를 수집하는 데 필요한 스키마를 관리하는 방법을 알아봅니다.
feature: Schemas
exl-id: 08289581-5af9-4422-b049-8c24105e2a8e
source-git-commit: 7524c2ffc0408b04e6bef5bd5deedc1feea0b682
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 4%

---

# 스키마

Experience Platform에서 수집하고 Mix Modeler에서 사용할 데이터를 지원하는 스키마를 관리하려면 다음을 수행하십시오.

1. Mix Modeler 인터페이스로 이동합니다.

1. ![&#x200B; 아래의 &#x200B;](/help/assets/icons/Schemas.svg)스키마&#x200B;**[!UICONTROL Schemas]** **[!UICONTROL SETUP]**&#x200B;을(를) 선택하십시오.

자세한 내용은 [스키마 UI 개요](https://experienceleague.adobe.com/docs/experience-platform/xdm/ui/overview.html?lang=ko)를 참조하십시오.

## 집계 또는 요약 데이터

XDM 요약 지표 클래스를 Experience Platform에서 수집하고 Mix Modeler에서 사용하려는 집계 또는 요약 데이터의 기본 스키마의 기반으로 사용하는 것이 좋습니다.

XDM 요약 지표 클래스 사용:

- 벽 정원 데이터 (예: Facebook 또는 YouTube 데이터)

- SPX(S&amp;P 500 주가 지수), 날씨 데이터 등의 외부 요인 데이터,

- 내부 요소 데이터(예: 가격 변경, 휴일 달력).

>[!IMPORTANT]
>
>수집된 데이터에 필요한 지표를 지원하려면 스키마 정의에 하나 이상의 숫자 필드(정수, Double, 부울 또는 기타 숫자 유형 사용)가 포함되어야 합니다.

아래 **[!DNL XDM Summary Metrics]**&#x200B;에 표시된 대로 **[!DNL ExternalFactorSummarySchema]** 기본 클래스를 사용하는 스키마는 간단할 수 있습니다.

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


**[!DNL LumaPaidMarketingSchema]**&#x200B;을(를) 기본 클래스로 사용하는 **[!DNL XDM Summary Metrics]**&#x200B;에 대한 보다 포괄적인 예제는 아래를 참조하십시오. 스키마는 지표(**[!DNL AMMMetrics]**), 차원(**[!DNL AMMDimensions]**) 및 기타 고객별 정보(**[!DNL CustomerSpecific]**)에 대해 색상 주석이 있는 전용 필드 그룹을 사용합니다.

![요약 스키마](/help/assets/summary-schema.png)

프로필 수집의 비동기적 특성을 고려할 때 외부 소스에서 합계 또는 요약 데이터를 수집할 때 외부 Source 시스템 감사 세부 정보 필드 그룹을 스키마의 일부로 사용하는 것이 좋습니다. 이 필드 그룹은 외부 소스에 대한 감사 속성 집합을 정의합니다.

## 요소 표준 필드 필드 그룹

편의상, Experience Platform은 내부 및 외부 요인 데이터(종종 요약, 내부 요인 또는 외부 요인 데이터의 일부)에 대한 전용 요인 표준 필드 필드 그룹을 지원합니다. 이 필드 그룹은 다음 필드를 정의합니다.

| 필드 표시 이름 | 필드 이름 | 필드 유형 | 데이터 유형 | 필수 여부 | 설명 |
|---|---|---|---|:-:|---|
| 요소 이름 | factorName | 차원 | 문자열 | ![확인 표시](/help/assets/icons/Checkmark.svg) | 계수의 이름입니다. |
| 요소 값 | factorValue | 지표 | Double | ![확인 표시](/help/assets/icons/Checkmark.svg) | 인자 값 |
| 요소 유형 | factorType | 차원 | 문자열(열거형) | | 인자의 유형입니다.<br/>가능한 값은 다음과 같습니다. <ul><li>내부(내부 계수)</li><li>외부(외부 요소)</li></ul> |
| 값 유형 | valueType | 차원 | 문자열(열거형) | | 가능한 값:<ul><li>실제(실제 값)</li><li>예측된(예측된 값)</li></ul>값이 없으면 실제 값이 기본값입니다. |
| 세부기간 | 세부기간 | 차원 | 문자열(열거형) | | 가능한 값:<ul><li>매일</li><li>매주</li><li>월별</li></ul> |

요약, 내부 요소 또는 외부 요소 데이터 세트는 다음을 기반으로 할 수 있습니다.

- 요소 표준 필드 그룹을 **사용**&#x200B;하는 스키마. 이 데이터 집합은 데이터 집합 규칙을 구성할 때 **[!UICONTROL Factors]** 데이터 집합으로 표시됩니다. 그리고 데이터 세트에 대한 데이터 세트 규칙의 일부로 정의하는 조화로운 필드는 모델을 만들 때 요소로 사용할 수 있습니다.
- **요소 표준 필드 그룹을 사용하지 않는** 스키마. 이 데이터 집합은 데이터 집합 규칙을 구성할 때 **[!UICONTROL Summary]** 데이터 집합으로 표시됩니다. 데이터 세트는 요약 데이터로 구성되며, 조화된 데이터에는 영향을 주지 않습니다.

## 지원되는 데이터 유형

현재 Mix Modeler은 Experience Platform 데이터 유형의 하위 집합을 지원합니다. [스키마 컴포지션의 기본 사항](https://experienceleague.adobe.com/docs/experience-platform/xdm/schema/composition.html?lang=ko#data-type)에 언급된 다음 기본 데이터 형식(필드)이 지원됩니다.

- 문자열
- 정수
- Double
- 부울
- 길게
- 짧음
- 바이트
- Date
- 날짜-시간


>[!MORELIKETHIS]
>
>- [스키마](schemas.md)
