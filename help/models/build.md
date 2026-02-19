---
title: Mix Modeler에서 모델 구축
description: 모델의 고급 옵션을 설정, 구성 및 지정하는 방법을 포함하여 Mix Modeler에서 모델을 구축하는 방법에 대해 알아봅니다.
feature: Models
solution: Mix Modeler
exl-id: e1093c09-1e23-460b-92de-cfb0061112fd
source-git-commit: 011b9b83569925ca9ff4f1ee472288473fbe8502
workflow-type: tm+mt
source-wordcount: '1276'
ht-degree: 2%

---

# 모델 구축

사용자 지정 AI 기반 모델을 구축하기 위해 인터페이스는 단계별 가이드 모델 구성 플로우를 제공합니다.

Mix Modeler의 ![모델](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** 인터페이스에서 **[!UICONTROL Open model canvas]**&#x200B;을(를) 선택합니다.

## 설정

**[!UICONTROL Setup]** 단계에서 이름 및 설명을 정의합니다.

1. **[!UICONTROL Name]** 모델(예: `Demo model`)을 입력하십시오. **[!UICONTROL Description]**(예: `Demo model to explore AI features of Mix Modeler`)을(를) 입력하십시오.

   ![모델 이름 및 설명](/help/assets/model-name-description.png)

1. 다음 단계로 진행하려면 **[!UICONTROL Next]**&#x200B;을(를) 선택하십시오. 모델 구성을 취소하려면 **[!UICONTROL Cancel]**&#x200B;을(를) 선택하십시오.

## 구성{#configure}

>[!CONTEXTUALHELP]
>id="model_marketingtouchpoints_select"
>title="마케팅 접점"
>abstract="마케팅 접점은 마케팅 투자가 수치적 또는 수익 기반 전환에 미치는 영향을 평가하는 데 사용되는 수신자, 개인 및 쿠키 수준의 마케팅 이벤트입니다.<br/><br/>데이터가 겹치는 터치포인트로 모델을 설정할 수 없으며 지출이 있는 터치포인트가 하나 이상 있어야 합니다."

**[!UICONTROL Configure]** 단계에서 모델을 구성합니다. 구성에는 전환 목표, 마케팅 접점, 적격 데이터 채우기, 외부 및 내부 요인 등의 정의가 포함됩니다.

1. **[!UICONTROL Conversion goal]** 섹션에서:

   ![모델 - 변환 단계](/help/assets/model-conversion-step.png)

   1. **[!UICONTROL Conversion]** 드롭다운 메뉴에서 전환을 선택합니다. 사용 가능한 전환은 [에서 ](../harmonize-data/conversions.md)전환[!UICONTROL Harmonized datasets]의 일부로 정의한 전환입니다. 예: **[!UICONTROL Online Conversion]**.

   1. 모델 구성 내에서 직접 변환을 만들려면 ![LinkOutLight](/help/assets/icons/LinkOutLight.svg) **[!UICONTROL Create a conversion]**&#x200B;을(를) 선택할 수 있습니다.



1. **[!UICONTROL Marketing touchpoints]** 섹션에서 [에 ](../harmonize-data/marketing-touchpoints.md)마케팅 접점[!UICONTROL Harmonized datasets]의 일부로 정의한 마케팅 접점에 해당하는 마케팅 접점을 하나 이상 선택할 수 있습니다.


   ![모델 - 마케팅 접점 단계](/help/assets/model-marketing-touchpoint-step.png)

   1. **[!UICONTROL Touchpoint include]** 드롭다운 메뉴에서 하나 이상의 마케팅 터치포인트를 선택합니다.

      * ![CrossSize75](/help/assets/icons/CrossSize75.svg)을(를) 사용하여 터치포인트를 제거할 수 있습니다.
      * **[!UICONTROL Clear all]**&#x200B;을(를) 사용하여 모든 터치포인트를 제거할 수 있습니다.

   1. ![LinkOutLight](/help/assets/icons/LinkOutLight.svg) **[!UICONTROL Create a touchpoint]**&#x200B;을(를) 선택하여 모델 구성 내에서 직접 마케팅 접점을 만들 수 있습니다.

   >[!NOTE]
   >
   >데이터가 겹치는 터치포인트로 모델을 설정할 수 없으며 지출이 있는 터치포인트가 하나 이상 있어야 합니다.

1. 기본적으로 점수는 사용자의 조화로운 보기에 있는 모든 데이터에 대해 생성됩니다. 모집단의 하위 집합에만 점수를 매기려면 **[!UICONTROL Eligible data population]** 섹션에서 컨테이너를 사용하여 하나 이상의 필터를 정의합니다.

   ![모델 - 적격 데이터 채우기](/help/assets/model-eligible-data-population-step.png)

   * 각 컨테이너에 대해 이벤트를 하나 이상 정의합니다.

      1. 각 이벤트에 대해:

         1. **[!UICONTROL _통합 필드 선택_]**&#x200B;에서 지표 또는 차원을 선택합니다.

         1. 적절한 연산자(**[!UICONTROL equals]**, **[!UICONTROL not equals]**, **[!UICONTROL less than]**, **[!UICONTROL greater than]**, **[!UICONTROL starts with]**, **[!UICONTROL doesn't start with]**, **[!UICONTROL ends with]**, **[!UICONTROL doesn't end with]**, **[!UICONTROL contains]**, **[!UICONTROL doesn't contain]**, **[!UICONTROL is in]** 또는 **[!UICONTROL is not in]**)를 선택하십시오.

         1. **[!UICONTROL _값을 입력하거나 선택하십시오_]**.

      1. 컨테이너에 이벤트를 추가하려면 ![추가](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add event]**&#x200B;을(를) 선택하십시오.

      1. 컨테이너에서 이벤트를 제거하려면 ![닫기](/help/assets/icons/CrossSize75.svg)를 선택합니다.

      1. 컨테이너에 정의된 모든 이벤트 또는 여러 이벤트를 사용하여 필터링하려면 **[!UICONTROL Any of]** 또는 **[!UICONTROL All of]**&#x200B;을(를) 선택합니다. 레이블이 **[!UICONTROL Include ... Or ...]**&#x200B;에서 **[!UICONTROL Include ... And ...]**(으)로 변경됩니다.

   * 적합한 데이터 채우기 컨테이너를 추가하려면 ![추가](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add eligible population]**&#x200B;을(를) 선택하십시오.

   * 적격한 데이터 채우기 컨테이너를 제거하려면 컨테이너 내에서 ![자세히](/help/assets/icons/More.svg)를 선택하고 상황에 맞는 메뉴에서 **[!UICONTROL Remove container]**&#x200B;을(를) 선택합니다.

   * 적격 데이터 모집단에 대해 보다 복잡한 정의를 만들려면 컨테이너 사이에 **And** 및 **Or**&#x200B;을(를) 선택하십시오.


1. 모델에 외부 요소가 포함된 데이터 세트를 추가하려면 **[!UICONTROL External factors dataset]** 섹션에서 하나 이상의 컨테이너를 사용하십시오. 외부요인의 예로 S&amp;P 지수를 들 수 있다.

   ![모델 - 외부 요인 데이터 세트](/help/assets/model-external-factors-dataset-step.png)

   * 각 컨테이너의 경우:

      1. **[!UICONTROL External factor name]**(예: `External Factors`)을(를) 입력하십시오.

      1. **[!UICONTROL Dataset]** 드롭다운 메뉴에서 데이터 세트를 선택합니다. 데이터 집합을 관리하려면 ![데이터](/help/assets/icons/Data.svg)를 선택할 수 있습니다. 자세한 내용은 [데이터 세트](../ingest-data/datasets.md)를 참조하십시오.

      1. **[!UICONTROL Impact on conversion]** 드롭다운 메뉴에서 옵션을 선택하십시오. **[!UICONTROL Auto select]**, **[!UICONTROL Positive]** 또는 **[!UICONTROL Negative]**. 기본 옵션은 모델이 영향을 결정할 수 있도록 하는 **[!UICONTROL Auto select]**&#x200B;입니다. 기본값을 재정의할 수 있습니다.

   * 추가 외부 요인 데이터 세트 컨테이너를 추가하려면 ![추가](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add external factor]**&#x200B;을(를) 선택하십시오.

   * 외부 요소 데이터 집합 컨테이너를 제거하려면 ![RemoveCircle](/help/assets/icons/RemoveCircle.svg)을(를) 선택하십시오.




1. 내부 요소가 포함된 데이터 세트를 모델에 추가하려면 **[!UICONTROL Internal factors dataset]** 섹션에서 하나 이상의 컨테이너를 사용하십시오. 내부 요인의 예로는 이메일 마케팅 데이터가 있습니다.

   ![모델 - 내부 요소 데이터 세트](/help/assets/model-internal-factors-dataset-step.png)

   * 각 컨테이너의 경우:

      1. **[!UICONTROL Internal factor name]**(예: `Email Marketing Data`)을(를) 입력하십시오.

      1. **[!UICONTROL _데이터 집합 선택_]**&#x200B;에서 데이터 집합을 선택하십시오. 데이터 집합을 관리하려면 ![데이터](/help/assets/icons/Data.svg)를 선택할 수 있습니다. 자세한 내용은 [데이터 세트](../ingest-data/datasets.md)를 참조하십시오.

      1. **[!UICONTROL Impact on conversion]** 드롭다운 메뉴에서 옵션을 선택하십시오. **[!UICONTROL Auto select]**, **[!UICONTROL Positive]** 또는 **[!UICONTROL Negative]**.

   * 추가 내부 요소 데이터 집합 컨테이너를 추가하려면 ![추가](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add internal factor]**&#x200B;을(를) 선택하십시오.

   * 내부 요소 데이터 집합 컨테이너를 제거하려면 ![RemoveCircle](/help/assets/icons/RemoveCircle.svg)을(를) 선택하십시오.



1. 모델에 대한 전환 확인 기간을 정의하려면 `1`에 `52`에서 **[!UICONTROL Give contribution credit to touchpoints occurring within]** 사이의 값을 입력하십시오. **[!UICONTROL weeks prior to the conversion]**.

1. 다음 단계로 진행하려면 **[!UICONTROL Next]**&#x200B;을(를) 선택하십시오. 추가 구성이 필요한 경우 빨간색 윤곽선과 텍스트가 추가 구성이 필요한 사항을 설명합니다. <br/>이전 단계로 돌아가려면 **[!UICONTROL Back]**&#x200B;을(를) 선택하십시오. <br/>모델 구성을 취소하려면 **[!UICONTROL Cancel]**&#x200B;을(를) 선택하십시오.


## 고급

**[!UICONTROL Advanced]** 단계에서 고급 설정을 지정할 수 있습니다. 이 단계에서는 멀티 터치 속성(MTA)에 대한 모델을 활성화할 수 있습니다.

1. **[!UICONTROL Spend share]** 섹션에서:

   * 과거 마케팅 투자 비율을 사용하여 마케팅 데이터가 희소할 때 모델을 알리려면 **[!UICONTROL Allow spend share]**&#x200B;을(를) 활성화합니다. 이 설정은 특히 다음 시나리오에서 권장됩니다.
      * 채널에 충분한 관찰이 없습니다(예: 지출 빈도가 낮거나 노출 횟수 또는 클릭 수).
      * 데이터가 희박할 수 있는 스파이크하지만 일반적이고 잠재적으로 비용이 높은 미디어(일부 브랜드의 TV 등)를 모델링합니다.

     >[!NOTE]
     >
     >일회성 투자(예: 슈퍼볼 광고)의 경우 점유율에 의존하기 보다는 해당 데이터를 요소로 통합하는 것이 좋습니다.
     >


1. **[!UICONTROL MTA enabled]** 섹션에서:

   * 모델에 대해 MTA 기능을 활성화하려면 **[!UICONTROL MTA enabled]**&#x200B;을(를) 활성화합니다. MTA를 활성화한 경우 멀티터치 속성 인사이트는 모델을 교육하고 점수를 매긴 후 사용할 수 있습니다. [모델 인사이트](insights.md#attribution)에서 [속성](insights.md) 탭을 참조하십시오.

1. **[!UICONTROL Prior knowledge]** 섹션에서:

   ![모델 - 사전 지식](/help/assets/model-prior-knowledge-step.png)

   1. 기본적으로 **[!UICONTROL Rule type]**&#x200B;인 **[!UICONTROL Absolute values]**&#x200B;을(를) 선택하십시오.

   1. **[!UICONTROL Name]** 열을 사용하여 **[!UICONTROL Contribution proportion]** 아래에 나열된 채널에 대한 기여도 백분율을 지정하십시오.

   1. 필요한 경우 각 채널에 대해 **[!UICONTROL Level of confidence]** 백분율을 추가할 수 있습니다.

   1. 필요한 경우 **[!UICONTROL Clear all]**&#x200B;을(를) 사용하여 **[!UICONTROL Contribution proportion]** 및 **[!UICONTROL Level of confidence]** 열에 대한 모든 입력 값을 지웁니다.


## 옵션 설정

[ 단계에서 ](#schedule)교육 및 채점을 예약[, ](#training-window)교육 기간을 정의[하고 모델에 대한 ](#granular-insights-reporting-fields)세부적인 통찰력 보고 필드&#x200B;**[!UICONTROL Set options]**&#x200B;를 지정할 수 있습니다.


### 일정

**[!UICONTROL Schedule]** 섹션에서 모델 교육 및 채점을 예약할 수 있습니다.

![일정 모델](../assets/model-schedule.png)

스케줄링된 모델 채점 및 교육을 수행하려면

1. **[!UICONTROL Enable scheduled model scoring and training]**&#x200B;을(를) 켭니다.
1. **[!UICONTROL Scoring frequency]** 선택:

   * **[!UICONTROL Daily]**: 올바른 시간(예: `05:22 pm`)을 입력하거나 ![시계](/help/assets/icons/Clock.svg)를 사용하십시오.
   * **[!UICONTROL Weekly]**: 요일을 선택하고 올바른 시간(예: `05:22 pm`)을 입력하거나 ![시계](/help/assets/icons/Clock.svg)를 사용하십시오.
   * **[!UICONTROL Monthly]**: 모든 드롭다운 메뉴에서 요일을 선택하고 올바른 시간(예: `05:22 pm`)을 입력하거나 ![시계](/help/assets/icons/Clock.svg)를 사용하십시오.

1. 드롭다운 메뉴에서 **[!UICONTROL Training frequency]**&#x200B;을(를) 선택합니다. **[!UICONTROL Monthly]**, **[!UICONTROL Quarterly]**, **[!UICONTROL Yearly]** 또는 **[!UICONTROL None]**.


### 교육 기간

**[!UICONTROL Define training window]** 섹션에서 다음 중 하나를 선택합니다.

![모델 - 교육 기간 정의](/help/assets/model-define-training-window.png)

* **[!UICONTROL Have Mix Modeler select a helpful training window]** 및

* **[!UICONTROL Manually input a training window]** 질문에 답합니다. 선택한 경우 **[!UICONTROL Include events the following years prior to a conversion]**&#x200B;의 연도 수를 정의합니다.


### 세분화된 통찰력 보고 필드

**[!UICONTROL Granular insights reporting fields]** 섹션은 세분화된 증분 보고 기능을 사용합니다. 이 기능을 사용하면 전환 및 접점 증분 점수를 분류하기 위해 조화된 필드를 선택할 수 있습니다.

![세부적인 인사이트 보고 필드 정의](/help/assets/granular-insights-reporting-fields.png)

별도의 모델을 생성하지 않고도 세분화된 보고 열을 사용하여 모델 보고에서 드릴다운할 수 있도록 이러한 통합 필드를 정의합니다.

예를 들어 매출에 중점을 둔 모델을 구축하지만 캠페인, 미디어 유형, 지역 및 트래픽 소스 성과에도 관심이 있습니다. 세분화된 증분 보고 기능이 없으면 네 개의 개별 모델을 빌드해야 합니다. 세분화된 증분 보고 기능을 사용하여 캠페인, 미디어 유형, 지역 및 트래픽 소스에 대한 수익 모델을 분류할 수 있습니다.

1. **[!UICONTROL _통합 필드 선택_]**&#x200B;에서 **[!UICONTROL Includes]** 아래의 통합 필드를 하나 이상 선택하십시오. 선택한 조화화된 필드가 패널에 추가됩니다.
1. **[!UICONTROL *Harmonized 필드&#x200B;*]**![CrossSize100](/help/assets/icons/CrossSize100.svg)을(를) 선택하여 선택된 Harmonized 필드가 있는 컨테이너에서 Harmonized 필드를 제거합니다.
1. **[!UICONTROL Clear all]**&#x200B;을(를) 선택하여 선택된 모든 조화 필드를 제거합니다.

세분화된 증분 보고를 위해 선택한 조화 필드는 모델을 채점한 결과 발생하는 Experience Platform [스키마](/help/ingest-data/schemas.md) 및 [데이터 세트](/help/ingest-data/datasets.md)의 일부로 사용할 수 있습니다. 세분화된 인사이트 보고 필드는 **[!UICONTROL conversionPassthrough]** 및 **[!UICONTROL touchpointPassthrough]** 개체 내에서 찾을 수 있습니다.

세분화된 증분 보고를 사용할 수 있는 모델의 스키마에 있는 ![conversionPassthrough 및 touchpointPassthrough 개체의 스크린샷](/help/assets/schema-granular-insights-reporting.png)


## 완료

* 모델 구성을 완료하려면 **[!UICONTROL Finish]**&#x200B;을(를) 선택하십시오.

   * **[!UICONTROL Create instance?]** 대화 상자에서 **[!UICONTROL Ok]**&#x200B;을(를) 선택하여 첫 번째 교육 및 채점 실행을 즉시 트리거합니다. 모델이 상태 ![StatusOrange](/help/assets/icons/StatusOrange.svg) **[!UICONTROL Awaiting training]**(으)로 나열됩니다.

     취소할 **[!UICONTROL Cancel]**&#x200B;을(를) 선택하십시오.

   * 추가 구성이 필요한 경우 빨간색 윤곽선과 텍스트가 추가 구성이 필요한 사항을 설명합니다.

* 이전 단계로 돌아가려면 **[!UICONTROL Back]**&#x200B;을(를) 선택하십시오.

* 모델 구성을 취소하려면 **[!UICONTROL Cancel]**&#x200B;을(를) 선택하십시오.

