---
title: 계획 수립
description: Mix Modeler에서 계획을 세우는 방법에 대해 알아봅니다.
feature: Plans
exl-id: 6d61d0b2-5871-4d00-9a35-73fff0a1c3e5
source-git-commit: 20985d0f9e9d2990b881ab448f6475e4bb8244d1
workflow-type: tm+mt
source-wordcount: '948'
ht-degree: 0%

---


# 계획 수립

Mix Modeler에서 계획 마법사를 사용하여 계획을 생성합니다. 계획 마법사에서 계획 및 계획에 사용할 기본 모델의 세부 정보 및 예산 또는 대상 지표를 설정할 수 있습니다. 세부 정보, 예산, 타겟 지표 및 모델을 지정했으면 AI 추천 플랜을 진행하거나 채널별 지출을 편집할 수 있습니다. 전환당 평균 매출액 및 채널 비용에 대한 고급 구성을 정의할 수 있습니다.

계획을 극대화할 목표를 정의해야 합니다. 이 목표는 지출할 수 있는 예산 또는 달성하고자 하는 목표가 될 수 있습니다. 목표가 목표인 경우 사용할 대상 지표에 대한 값(전환, 매출, CPA 또는 ROI)을 추가로 지정해야 합니다.

계획을 만들려면 Mix Modeler의 ![PLan](/help/assets/icons/FileChart.svg) **[!UICONTROL Plans]** 인터페이스에서 **[!UICONTROL Create plan]**&#x200B;을(를) 선택하십시오.


1. **[!UICONTROL Plan creation]** 화면에서 다음을 수행합니다.

   1. **[!UICONTROL Setup]** 섹션에서:

      1. **[!UICONTROL Plan name]**(예: `Goal based plan`)을(를) 입력하십시오. **[!UICONTROL Description]**(예: `A goal based plan`)을(를) 입력하십시오.
      1. **[!UICONTROL Model]**&#x200B;에서 **[!UICONTROL _을(를) 선택하십시오. 옵션을 선택하십시오._.]**

         ![계획 설정](/help/assets/plan-setup.png)

   1. **[!UICONTROL Goal]** 섹션에서 계획을 최적화할 목표를 선택합니다. 다음 중 하나를 선택할 수 있습니다.

      * **[!UICONTROL I have a budget to spend]**

        ![계획 예산](../assets/plan-budget.png)

        이 옵션을 사용하면 하나 이상의 날짜 범위에 대한 예산을 입력할 수 있습니다.

         1. **[!UICONTROL Optimize]** 컨테이너에서:
            1. **[!UICONTROL Select conversion]** 드롭다운 메뉴에서 전환을 선택합니다.
            1. **[!UICONTROL Select model]** 드롭다운 메뉴에서 모델을 선택합니다.
         1. 날짜를 입력하거나 **[!UICONTROL Date range]**&#x200B;달력![을 사용하여 날짜 범위를 선택하여 ](/help/assets/icons/Calendar.svg)을(를) 지정하십시오.
         1. **[!UICONTROL Budget]** 입력.
각각 예산이 있는 날짜 범위를 추가하려면 ![CalendarAdd](/help/assets/icons/CalendarAdd.svg) **[!UICONTROL Add row]**을(를) 선택하십시오.
날짜 범위 및 관련 예산을 삭제하려면 ![닫기](/help/assets/icons/Close.svg)를 선택하세요.
         1. 계획을 제한하려는 선택적 최대 예산을 정의하려면
            1. **[!UICONTROL Maximize budget]** 스위치를 켭니다.
            1. 최대 예산 금액을 지정합니다. 금액은 날짜 범위에 대해 지정된 예산의 총 금액보다 크거나 같아야 합니다.


      * **[!UICONTROL I have a target to achieve]** [!BADGE Beta]

        ![대상 계획](../assets/plan-target.png)

         1. **[!UICONTROL Optimize]** 컨테이너에서
            1. **[!UICONTROL Select conversion]** 드롭다운 메뉴에서 전환을 선택합니다.
            1. **[!UICONTROL Select target metric]** 드롭다운 메뉴에서 대상 지표를 선택합니다. **[!UICONTROL Conversion]**, **[!UICONTROL CPA]**, **[!UICONTROL Revenue]** 또는 **[!UICONTROL ROI]** 중에서 선택할 수 있습니다.
            1. **[!UICONTROL Select model]** 드롭다운 메뉴에서 모델을 선택합니다.
         1. 날짜를 입력하거나 ![달력](/help/assets/icons/Calendar.svg)을 사용하여 날짜 범위를 선택하여 날짜 범위를 지정하십시오.
         1. 선택한 대상 지표에 대한 값을 입력합니다. 예를 들어, **[!UICONTROL Total Conversions]**&#x200B;의 숫자, **[!UICONTROL Paid Marketing ROI]**&#x200B;의 백분율 또는 **[!UICONTROL Paid Marketing CPA]** 및 **[!UICONTROL Total Revenue]**의 통화 값입니다.
대상 지표가 있는 날짜 범위를 추가하려면 ![CalendarAdd](/help/assets/icons/CalendarAdd.svg) **[!UICONTROL Add row]**을(를) 선택하십시오.
날짜 범위 및 연결된 대상 지표를 삭제하려면 ![닫기](/help/assets/icons/Close.svg)를 선택하세요.
         1. 계획을 제한하려는 선택적 최대 예산을 정의하려면
            1. **[!UICONTROL Maximize budget]** 스위치를 켭니다.
            1. 최대 예산 금액을 지정합니다.


   1. **[!UICONTROL Next]**&#x200B;를 선택합니다.

1. **[!UICONTROL Done with all required fields]** 대화 상자에서:

   ![계획 완료](/help/assets/plan-done-required-fields.png)

   * 예측된 ROI가 포함된 AI 추천 플랜을 생성하려면 ![새 플랜](/help/assets/icons/NewPlan.svg) **[!UICONTROL Create plan now]**&#x200B;을(를) 선택하십시오. **[!UICONTROL OK]**&#x200B;을(를) 선택합니다. 플랜이 생성되었습니다.





   * 예측된 ROI가 있는 계획을 만들기 전에 채널 예산을 편집하고 고급 구성을 정의하려면 ![테이블 편집](/help/assets/icons/TableEdit.svg) **[!UICONTROL Edit channel budgets first]**&#x200B;을(를) 선택하십시오.  다음 단계에서 **[!UICONTROL OK]**&#x200B;에서 채널 지출을 정의할 수 있도록 **[!UICONTROL Spend selection]**&#x200B;을(를) 선택하십시오.


     >[!IMPORTANT]
     >
     >아래 정보는 ![TableEdit](/help/assets/icons/TableEdit.svg) **[!UICONTROL Edit channel budgets first]**&#x200B;을(를) 선택한 경우에만 관련이 있습니다.


1. **[!UICONTROL Spend selection]** 섹션에서 각 예산 날짜 범위에 대해 ![V자형 화살표](/help/assets/icons/ChevronRight.svg)를 사용하여 해당 데이터 범위에 대한 채널 배포 보기를 엽니다.

   과거 마케팅 지출 데이터와 통찰력을 사용하려는 경우 내역 참조 데이터를 사용할 수 있습니다. 내역 참조 데이터를 고려하십시오.

   * 성과가 좋은 채널과 성과가 나쁜 채널을 강조 표시하여 예산 할당을 개선합니다.
   * 지원 트렌드 분석.
   * 효과적인 전략을 식별하고 계획을 구성하는 동안 실수를 방지합니다.

   과거 참조 기간을 선택하는 경우 이전 지출 패턴 환경 설정에 맞게 조정하며 Mix Modeler의 계획 기능을 사용하면 예상 범위 내의 계획을 생성할 수 있습니다. 이러한 플랜은 궁극적으로 관련자의 신뢰를 강화하고, 마케팅 플랜이 전략적이고 효율적이며, 이러한 플랜이 입증된 성과 데이터 및 비즈니스 요구에 기반을 두도록 해야 합니다.

   ![선택 비용](/help/assets/plan-spend-selection.png)

   1. **[!UICONTROL Spend pattern]**&#x200B;을(를) 선택합니다.

      * 기본 옵션은 **[!UICONTROL Automatic]**&#x200B;입니다.
      * Mix Modeler에서 이미 사용 가능한 과거 마케팅 지출 데이터를 참조하려면 **[!UICONTROL Historical reference]**&#x200B;을(를) 선택하고 **[!UICONTROL Start date]**&#x200B;을(를) 입력하십시오. **[!UICONTROL End date]**&#x200B;은(는) 지출 패턴을 정의하는 날짜 범위를 기반으로 자동으로 결정됩니다. 제안된 시작 날짜는 사용 가능한 첫 번째 사용 가능한 과거 마케팅 지출 날짜입니다. 존재하지 않거나 잘못된 기록 참조 기간을 선택했음을 나타내려면 ![AlertRed](/help/assets/icons/AlertRed.svg)가 표시됩니다.

   1. 각 채널의 예산을 정의하려면 **[!UICONTROL Min]** 및 **[!UICONTROL Max]**&#x200B;의 값을 입력하거나 슬라이더를 사용하십시오.

   1. 통화 또는 백분율 입력 간을 전환하려면 **[!UICONTROL $]**&#x200B;에 대해 **[!UICONTROL %]** 또는 **[!UICONTROL View spend by]**&#x200B;을(를) 선택하세요. 통화 기반이 아닌 대상 지표를 선택한 경우 이 토글이 비활성화됩니다.

   1. 완료되면 **[!UICONTROL Create]**을(를) 선택합니다.
      ![선택 비용](/help/assets/plan-spend-selection.png)

   1. **[!UICONTROL Next]**&#x200B;를 선택합니다.



1. **[!UICONTROL Advanced configurations]** 섹션에서 선택적 고급 구성을 입력할 수 있습니다.

   ![계획 요약](../assets/plan-advanced-configurations.png)

   * 계획명 , 모델, 날짜 범위 및 총 예산이 요약됩니다.

   * 기본적으로 Mix Modeler은 최신 이전 시즌 데이터를 사용하여 전환당 평균 매출을 자동으로 계산합니다. **[!UICONTROL Average Revenue per conversion]**&#x200B;에서 전환당 특정 평균 매출을 정의할 수 있습니다.

      1. 예산의 각 일자 범위에 대해

         1. **[!UICONTROL Date range]** 드롭다운 메뉴에서 날짜 범위를 선택합니다.
         1. **[!UICONTROL Average revenue]** 값을 입력하십시오.

      1. ![AddCircle](/help/assets/icons/AddCircle.svg) 전환 단위당 사용자 지정 평균 수익 추가를 선택하여 날짜 범위를 추가합니다.
      1. 날짜 범위를 제거하려면 ![RemoveCircle](/help/assets/icons/RemoveCircle.svg)을(를) 선택하십시오.

     >[!NOTE]
     >
     >모델에 이전 수익 데이터가 포함되지 않은 경우 예산에 대해 지정한 각 날짜 범위에 대해 전환당 평균 수익을 정의해야 합니다.
     >

   * 기본적으로 Mix Modeler은 최신 시즌 데이터를 사용하여 채널 비용을 자동으로 계산합니다. **[!UICONTROL Channel costs]**&#x200B;에서 사용자 지정 채널 비용을 정의할 수 있습니다.

      1. 모델의 각 채널에 대해 사용자 지정 채널 비용을 정의합니다.

         1. **[!UICONTROL Channel]** 드롭다운 메뉴에서 채널을 선택합니다.
         1. 예산의 각 일자 범위에 대해
            1. **[!UICONTROL Date range]** 드롭다운 메뉴에서 날짜 범위를 선택합니다.
            1. **[!UICONTROL Average revenue]** 값을 입력하십시오.
         1. 날짜 범위를 추가하려면 ![AddCircle](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add custom average revenue per conversion unit]**&#x200B;을(를) 선택하십시오.
         1. 날짜 범위를 제거하려면 ![RemoveCircle](/help/assets/icons/RemoveCircle.svg)을(를) 선택하십시오.

      1. 채널을 추가하려면 ![AddCircle](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add custom channel cost]**&#x200B;을(를) 선택하십시오.
      1. 사용자 지정 채널을 제거하려면 ![CrossSize400](/help/assets/icons/CrossSize400.svg)을(를) 선택하십시오.


1. 완료되면 **[!UICONTROL Create]**&#x200B;을(를) 선택합니다.

1. **[!UICONTROL Create plan]** 대화 상자에서 **[!UICONTROL Create plan]**&#x200B;을(를) 선택하여 계획을 만듭니다. **[!UICONTROL Cancel]**&#x200B;을(를) 선택하여 플랜 만들기를 취소하세요. 확인을 위해 **[!UICONTROL No work is saved]** 대화 상자가 표시됩니다.

