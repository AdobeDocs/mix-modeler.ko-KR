---
title: 모델 만들기
description: Mix Modeler에서 모델을 만드는 방법을 알아봅니다.
feature: Models
exl-id: e1093c09-1e23-460b-92de-cfb0061112fd
source-git-commit: ab3b5b4177fff324d50463210724ef95db18e67f
workflow-type: tm+mt
source-wordcount: '884'
ht-degree: 0%

---

# 모델 만들기

모델을 만들려면 Mix Modeler의 ![모델](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** 인터페이스에서 **[!UICONTROL Open model canvas]**&#x200B;을(를) 선택하십시오.

사용자 지정 AI 기반 모델을 구축하기 위해 인터페이스는 단계별 가이드 모델 구성 플로우를 제공합니다.

## 설정

**[!UICONTROL Setup]** 단계에서 이름과 설명을 정의합니다.

1. **[!UICONTROL Name]** 모델(예: `Demo model`)을 입력하십시오. **[!UICONTROL Description]**(예: `Demo model to explore AI featues of Mix Modeler`)을(를) 입력하십시오.

   ![모델 이름 및 설명](/help/assets/model-name-description.png)

1. 다음 단계로 진행하려면 **[!UICONTROL Next]**&#x200B;을(를) 선택하십시오. 모델 구성을 취소하려면 **[!UICONTROL Cancel]**&#x200B;을(를) 선택하십시오.

## 구성

**[!UICONTROL Configure]** 단계에서 모델을 구성합니다. 구성에는 전환 목표, 마케팅 접점, 적격 데이터 채우기, 외부 및 내부 요인 등의 정의가 포함됩니다.

1. **[!UICONTROL Conversion goal]** 섹션에서:

   ![모델 - 변환 단계](/help/assets/model-conversion-step.png)

   1. **[!UICONTROL Conversion]** 드롭다운 메뉴에서 전환을 선택합니다. 사용 가능한 전환은 [!UICONTROL Harmonized datasets]에서 [전환](../harmonize-data/conversions.md)의 일부로 정의한 전환입니다. 예: **[!UICONTROL Online Conversion]**.

   1. 모델 구성 내에서 직접 변환을 만들려면 ![LinkOutLight](/help/assets/icons/LinkOutLight.svg) **[!UICONTROL Create a conversion]**&#x200B;을(를) 선택할 수 있습니다.



1. **[!UICONTROL Marketing touchpoints]** 섹션에서 [!UICONTROL Harmonized datasets]에 [마케팅 접점](../harmonize-data/marketing-touchpoints.md)의 일부로 정의한 마케팅 접점에 해당하는 마케팅 접점을 하나 이상 선택할 수 있습니다.


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

   * 적격한 데이터 채우기 컨테이너를 제거하려면 컨테이너 내에서 ![자세히](/help/assets/icons/More.svg)를 선택하고 상황에 맞는 메뉴에서 **[!UICONTROL Remove marketing touchpoint]**&#x200B;을(를) 선택합니다.



1. 모델에 외부 요소가 포함된 데이터 세트를 추가하려면 **[!UICONTROL External factors dataset]** 섹션에서 하나 이상의 컨테이너를 사용하십시오. 외부요인의 예로 S&amp;P 지수를 들 수 있다.

   ![모델 - 외부 요인 데이터 세트](/help/assets/model-external-factors-dataset-step.png)

   * 각 컨테이너의 경우:

      1. **[!UICONTROL External factor name]**(예: `External Factors`)을(를) 입력하십시오.

      1. **[!UICONTROL Dataset]** 드롭다운 메뉴에서 데이터 세트를 선택합니다. 데이터 집합을 관리하려면 ![데이터](/help/assets/icons/Data.svg)를 선택할 수 있습니다. 자세한 내용은 [데이터 세트](../ingest-data/datasets.md)를 참조하십시오.

      1. **[!UICONTROL Impact on conversion]** 드롭다운 메뉴에서 옵션을 선택하십시오. **[!UICONTROL Auto select]**, **[!UICONTROL Positive]** 또는 **[!UICONTROL Negative]**.

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



1. 모델에 대한 전환 확인 기간을 정의하려면 **[!UICONTROL Give contribution credit to touchpoints occurring within]**&#x200B;에 `1`에서 `52` 사이의 값을 입력하십시오. **[!UICONTROL weeks prior to the conversion]**.

1. 다음 단계로 진행하려면 **[!UICONTROL Next]**&#x200B;을(를) 선택하십시오. 추가 구성이 필요한 경우 빨간색 윤곽선과 텍스트가 추가 구성이 필요한 사항을 설명합니다. <br/>이전 단계로 돌아가려면 **[!UICONTROL Back]**&#x200B;을(를) 선택하십시오. <br/>모델 구성을 취소하려면 **[!UICONTROL Cancel]**&#x200B;을(를) 선택하십시오.


## 고급

**[!UICONTROL Advanced]** 단계에서 고급 설정을 지정할 수 있습니다. 이 단계에서는 멀티 터치 속성(MTA)에 대한 모델을 활성화할 수 있습니다.

1. **[!UICONTROL Spend share]** 섹션에서:

   * 과거 마케팅 투자 비율을 사용하여 마케팅 데이터가 희소할 때 모델을 알리려면 **[!UICONTROL Allow spend share]**&#x200B;을(를) 활성화합니다.

1. **[!UICONTROL MTA enabled]** 섹션에서:

   * 모델에 대해 MTA 기능을 활성화하려면 **[!UICONTROL MTA enabled]**&#x200B;을(를) 활성화합니다. MTA를 활성화한 경우 멀티터치 속성 인사이트는 모델을 교육하고 점수를 매긴 후 사용할 수 있습니다. [모델 인사이트](insights.md)에서 [속성](insights.md#attribution) 탭을 참조하십시오.

1. **[!UICONTROL Prior knowledge]** 섹션에서:

   ![모델 - 사전 지식](/help/assets/model-prior-knowledge-step.png)

   1. 기본적으로 **[!UICONTROL Absolute values]**&#x200B;인 **[!UICONTROL Rule type]**&#x200B;을(를) 선택하십시오.

   1. **[!UICONTROL Contribution proportion]** 열을 사용하여 **[!UICONTROL Name]** 아래에 나열된 채널에 대한 기여도 백분율을 지정하십시오.

   1. 필요한 경우 각 채널에 대해 **[!UICONTROL Level of confidence]** 백분율을 추가할 수 있습니다.

   1. 필요한 경우 **[!UICONTROL Clear all]**&#x200B;을(를) 사용하여 **[!UICONTROL Contribution proportion]** 및 **[!UICONTROL Level of confidence]** 열에 대한 모든 입력 값을 지웁니다.


## 일정

**[!UICONTROL Schedule]** 단계에서 모델에 대한 교육 및 채점을 예약할 수 있습니다.

1. **[!UICONTROL Schedule]** 섹션에서 모델 교육 및 채점을 예약할 수 있습니다.

   ![일정 모델](../assets/model-schedule.png)

   스케줄링된 모델 채점 및 교육을 수행하려면

   1. **[!UICONTROL Enable scheduled model scoring and training]**&#x200B;을(를) 켭니다.
   1. **[!UICONTROL Scoring frequency]** 선택:

      * **[!UICONTROL Daily]**: 올바른 시간(예: `05:22 pm`)을 입력하거나 ![시계](/help/assets/icons/Clock.svg)를 사용하십시오.
      * **[!UICONTROL Weekly]**: 요일을 선택하고 올바른 시간(예: `05:22 pm`)을 입력하거나 ![시계](/help/assets/icons/Clock.svg)를 사용하십시오.
      * **[!UICONTROL Monthly]**: 모든 드롭다운 메뉴에서 요일을 선택하고 올바른 시간(예: `05:22 pm`)을 입력하거나 ![시계](/help/assets/icons/Clock.svg)를 사용하십시오.

   1. 드롭다운 메뉴에서 **[!UICONTROL Training frequency]**&#x200B;을(를) 선택합니다. **[!UICONTROL Monthly]**, **[!UICONTROL Quarterly]**, **[!UICONTROL Yearly]** 또는 **[!UICONTROL None]**.

1. **[!UICONTROL Define training window]** 섹션에서 다음 중 하나를 선택합니다.

   ![모델 - 교육 기간 정의](/help/assets/model-define-training-window.png)

   * **[!UICONTROL Have Mix Modeler select a helpful training window]** 및

   * **[!UICONTROL Manually input a training window]** 질문에 답합니다. 선택한 경우 **[!UICONTROL Include events the following years prior to a conversion]**&#x200B;의 연도 수를 정의합니다.


1. 모델 구성을 완료하려면 **[!UICONTROL Finish]**&#x200B;을(를) 선택하십시오.

   * **[!UICONTROL Create instance?]** 대화 상자에서 **[!UICONTROL Ok]**&#x200B;을(를) 선택하여 첫 번째 교육 및 채점 실행을 즉시 트리거합니다. 모델이 상태 ![StatusOrange](/help/assets/icons/StatusOrange.svg) **[!UICONTROL Awaiting training]**(으)로 나열됩니다.

     취소할 **[!UICONTROL Cancel]**&#x200B;을(를) 선택하십시오.

   * 추가 구성이 필요한 경우 빨간색 윤곽선과 텍스트가 추가 구성이 필요한 사항을 설명합니다.

   이전 단계로 돌아가려면 **[!UICONTROL Back]**&#x200B;을(를) 선택하십시오.

   모델 구성을 취소하려면 **[!UICONTROL Cancel]**&#x200B;을(를) 선택하십시오.
