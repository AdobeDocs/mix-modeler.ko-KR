---
title: 모델 만들기
description: Mix Modeler에서 모델을 만드는 방법을 알아봅니다.
feature: Models
exl-id: e1093c09-1e23-460b-92de-cfb0061112fd
source-git-commit: 9a6c1f1c12ab29da80a1997cfd31ca07b38eaa22
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 0%

---

# 모델 만들기

모델을 만들려면 Mix Modeler의 ![모델](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** 인터페이스에서 **[!UICONTROL Open model canvas]**&#x200B;을(를) 선택하십시오.

사용자 지정 AI 기반 모델을 구축하기 위해 인터페이스는 단계별 가이드 모델 구성 플로우를 제공합니다.

1. **[!UICONTROL Setup]** 단계:

   1. **[!UICONTROL Name]** 모델(예: `Demo model`)을 입력하십시오. **[!UICONTROL Description]**(예: `Demo model to explore AI featues of Mix Modeler`)을(를) 입력하십시오.

      ![모델 이름 및 설명](/help/assets/model-name-description.png)

   1. 다음 단계로 진행하려면 **[!UICONTROL Next]**&#x200B;을(를) 선택하십시오. 모델 구성을 취소하려면 **[!UICONTROL Cancel]**&#x200B;을(를) 선택하십시오.

1. **[!UICONTROL Configure]** 단계:

   1. **[!UICONTROL Conversion goal]** 섹션의 컨테이너 내에서 다음을 수행합니다.

      1. 변환을 위한 **[!UICONTROL Conversion name]**(예: `Conversion`)을(를) 입력하십시오.

      1. [!UICONTROL Harmonized datasets]에서 [전환](../harmonize-data/conversions.md)의 일부로 정의한 사용 가능한 전환이 포함된 **[!UICONTROL *통합 필드 선택&#x200B;*]**에서 전환을 선택하십시오. 예:**[!UICONTROL Online Conversion]**.

      1. 모델 구성 내에서 직접 전환을 만들려면 ![회신](/help/assets/icons/Reply.svg) **[!UICONTROL Create new conversion]**&#x200B;을(를) 선택할 수 있습니다.

         ![모델 - 변환 단계](/help/assets/model-conversion-step.png)

   1. **[!UICONTROL Marketing touchpoints]** 섹션에는 [!UICONTROL Harmonized datasets]에서 [마케팅 접점](../harmonize-data/marketing-touchpoints.md)의 일부로 정의한 마케팅 접점에 해당하는 많은 마케팅 접점 컨테이너가 표시됩니다.

      * 각 컨테이너의 경우:

         1. **[!UICONTROL Marketing touchpoint name]**&#x200B;을(를) 수정할 수 있습니다.

         1. **[!UICONTROL _마케팅 접점 선택_]**&#x200B;에서 마케팅 접점을 선택하십시오.

         1. ![회신](/help/assets/icons/Reply.svg) **[!UICONTROL Create new marketing touchpoint]**&#x200B;을(를) 선택하여 모델 구성 내에서 직접 마케팅 접점을 만들 수 있습니다.

      * 마케팅 접점 컨테이너를 추가하려면 ![추가](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add marketing touchpoint]**&#x200B;을(를) 선택하십시오.

      * 마케팅 접점 컨테이너를 제거하려면 컨테이너 내에서 ![자세히](/help/assets/icons/More.svg)를 선택하고 컨텍스트 메뉴에서 **[!UICONTROL Remove container]**&#x200B;을(를) 선택합니다.

        ![모델 - 마케팅 접점-단계](/help/assets/model-marketing-touchpoint-step.png)

   1. 기본적으로 점수는 사용자의 조화로운 보기에 있는 모든 데이터에 대해 생성됩니다. 모집단의 하위 집합에만 점수를 매기려면 **[!UICONTROL Eligible data population]** 섹션에서 컨테이너를 사용하여 하나 이상의 필터를 정의합니다.

      * 각 컨테이너에 대해 이벤트를 하나 이상 정의합니다.

         1. 각 이벤트에 대해:

            1. **[!UICONTROL _통합 필드 선택_]**&#x200B;에서 지표 또는 차원을 선택합니다.

            1. 적절한 연산자(**[!UICONTROL equals]**, **[!UICONTROL not equals]**, **[!UICONTROL less than]**, **[!UICONTROL greater than]**, **[!UICONTROL starts with]**, **[!UICONTROL doesn't start with]**, **[!UICONTROL ends with]**, **[!UICONTROL doesn't end with]**, **[!UICONTROL contains]**, **[!UICONTROL doesn't contain]**, **[!UICONTROL is in]** 또는 **[!UICONTROL is not in]**)를 선택하십시오.

            1. **[!UICONTROL _값을 입력하거나 선택하십시오_]**.

         1. 컨테이너에 이벤트를 추가하려면 ![추가](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add event]**&#x200B;을(를) 선택하십시오.

         1. 컨테이너에서 이벤트를 제거하려면 ![닫기](/help/assets/icons/Close.svg)를 선택합니다.

         1. 컨테이너에 정의된 모든 이벤트 또는 여러 이벤트를 사용하여 필터링하려면 **[!UICONTROL Any of]** 또는 **[!UICONTROL All of]**&#x200B;을(를) 선택합니다. 레이블이 **[!UICONTROL Include ... Or ...]**&#x200B;에서 **[!UICONTROL Include ... And ...]**(으)로 변경됩니다.

      * 적합한 데이터 채우기 컨테이너를 추가하려면 ![추가](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add eligible population]**&#x200B;을(를) 선택하십시오.

      * 적격한 데이터 채우기 컨테이너를 제거하려면 컨테이너 내에서 ![자세히](/help/assets/icons/More.svg)를 선택하고 상황에 맞는 메뉴에서 **[!UICONTROL Remove marketing touchpoint]**&#x200B;을(를) 선택합니다.

        ![모델 - 적격 데이터 채우기](/help/assets/model-eligible-data-population-step.png)

   1. 모델에 외부 요소가 포함된 데이터 세트를 추가하려면 **[!UICONTROL External factors dataset]** 섹션에서 하나 이상의 컨테이너를 사용하십시오.

      * 각 컨테이너의 경우:

         1. **[!UICONTROL _요소 입력_]**&#x200B;에 **[!UICONTROL Factor name]**&#x200B;을(를) 입력하십시오.

         1. **[!UICONTROL _데이터 집합 선택_]**&#x200B;에서 데이터 집합을 선택하십시오. 데이터 집합을 관리하려면 ![데이터](/help/assets/icons/Data.svg)를 선택할 수 있습니다. 자세한 내용은 [데이터 세트](../ingest-data/datasets.md)를 참조하십시오.

      * 추가 외부 요인 데이터 세트 컨테이너를 추가하려면 ![추가](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add external factor]**&#x200B;을(를) 선택하십시오.

      * 외부 요인 데이터 세트 컨테이너를 제거하려면 컨테이너 내에서 ![자세히](/help/assets/icons/More.svg)를 선택하고 컨텍스트 메뉴에서 **[!UICONTROL Remove external factor]**&#x200B;을(를) 선택합니다.

        ![모델 - 외부 요인 데이터 세트](/help/assets/model-external-factors-dataset-step.png)


   1. 내부 요소가 포함된 데이터 세트를 모델에 추가하려면 **[!UICONTROL Internal factors dataset]** 섹션에서 하나 이상의 컨테이너를 사용하십시오.

      * 각 컨테이너의 경우:

         1. **[!UICONTROL _요소 입력_]**&#x200B;에 **[!UICONTROL Factor name]**&#x200B;을(를) 입력하십시오.

         1. **[!UICONTROL _데이터 집합 선택_]**&#x200B;에서 데이터 집합을 선택하십시오. 데이터 집합을 관리하려면 ![데이터](/help/assets/icons/Data.svg)를 선택할 수 있습니다. 자세한 내용은 [데이터 세트](../ingest-data/datasets.md)를 참조하십시오.

      * 추가 내부 요소 데이터 집합 컨테이너를 추가하려면 ![추가](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add internal factor]**&#x200B;을(를) 선택하십시오.

      * 추가 내부 요소 데이터 세트 컨테이너를 제거하려면 컨테이너 내에서 컨텍스트 메뉴에서 ![자세히](/help/assets/icons/More.svg) 및 **[!UICONTROL Remove internal factor]**&#x200B;을(를) 선택합니다.

        ![모델 - 내부 요소 데이터 세트](/help/assets/model-internal-factors-dataset-step.png)

   1. 모델에 대한 전환 확인 기간을 정의하려면 **[!UICONTROL Give contribution credit to touchpoints occurring within]**&#x200B;에 `1`에서 `52` 사이의 값을 입력하십시오. **[!UICONTROL weeks prior to the conversion]**.

   1. 다음 단계로 진행하려면 **[!UICONTROL Next]**&#x200B;을(를) 선택하십시오. 추가 구성이 필요한 경우 빨간색 윤곽선과 텍스트가 추가 구성이 필요한 사항을 설명합니다. <br/>이전 단계로 돌아가려면 **[!UICONTROL Back]**&#x200B;을(를) 선택하십시오. <br/>모델 구성을 취소하려면 **[!UICONTROL Cancel]**&#x200B;을(를) 선택하십시오.

1. **[!UICONTROL Advanced]** 단계:

   1. **[!UICONTROL Define training window]** 섹션에서 다음 중 하나를 선택합니다.

      * **[!UICONTROL Have Mix Modeler select a helpful training window]** 및

      * **[!UICONTROL Manually input a training window]** 질문에 답합니다. 선택한 경우 **[!UICONTROL Include events the following years prior to a conversion]**&#x200B;의 연도 수를 정의합니다.

        ![모델 - 교육 기간 정의](/help/assets/model-define-training-window.png)

   1. **[!UICONTROL Spend share]** 섹션에서:

      * 과거 마케팅 투자 비율을 사용하여 마케팅 데이터가 희소할 때 모델을 알리려면 **[!UICONTROL Allow spend share]**&#x200B;을(를) 활성화합니다.

   1. **[!UICONTROL Prior knowledge]** 섹션에서:

      1. **[!UICONTROL Rule type]**&#x200B;을(를) 선택합니다.

      1. **[!UICONTROL Contribution proportion]** 열을 사용하여 **[!UICONTROL Name]** 아래에 나열된 채널에 대한 기여도 백분율을 지정하십시오.

      1. 필요한 경우 각 채널에 대해 **[!UICONTROL Level of confidence]** 백분율을 추가할 수 있습니다.

      1. 필요한 경우 **[!UICONTROL Clear all]**&#x200B;을(를) 사용하여 **[!UICONTROL Contribution proportion]** 및 **[!UICONTROL Level of confidence]** 열에 대한 모든 입력 값을 지웁니다.

         ![모델 - 사전 지식](/help/assets/model-prior-knowledge-step.png)

1. 모델 구성을 완료하려면 **[!UICONTROL Finish]**&#x200B;을(를) 선택하십시오.

   * **[!UICONTROL Create instance?]** 대화 상자에서 **[!UICONTROL Ok]**&#x200B;을(를) 선택하여 첫 번째 교육 및 채점 실행을 즉시 트리거합니다. 모델이 <span style="color:orange">●</span> 상태로 나열됩니다. **[!UICONTROL Awaiting training]**.

     취소할 **[!UICONTROL Cancel]**&#x200B;을(를) 선택하십시오.

   * 추가 구성이 필요한 경우 빨간색 윤곽선과 텍스트가 추가 구성이 필요한 사항을 설명합니다.

   이전 단계로 돌아가려면 **[!UICONTROL Back]**&#x200B;을(를) 선택하십시오.

   모델 구성을 취소하려면 **[!UICONTROL Cancel]**&#x200B;을(를) 선택하십시오.
