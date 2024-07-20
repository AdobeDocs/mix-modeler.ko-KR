---
title: 계획 만들기
description: Mix Modeler에서 계획을 만드는 방법을 알아봅니다.
feature: Plans
exl-id: 6d61d0b2-5871-4d00-9a35-73fff0a1c3e5
source-git-commit: 9085363e951a4e306c64ad28f56e2c15b4a6029a
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---


# 계획 만들기

Mix Modeler에서 계획 캔버스를 사용하여 계획을 생성합니다. 계획 캔버스에서 계획에 사용할 기본 모델과 계획의 세부 정보와 예산을 설정할 수 있습니다. 세부 정보, 예산 및 모델을 지정하면 AI 추천 플랜을 진행하거나 채널별 지출을 편집할 수 있습니다.

계획을 만들려면 Mix Modeler의 ![PLan](/help/assets//icons/FileChart.svg) **[!UICONTROL Plans]** 인터페이스에서 **[!UICONTROL Open plan canvas]**&#x200B;을(를) 선택하십시오.

1. 계획 생성 화면에서 다음을 수행합니다.

   1. **[!UICONTROL Setup]** 섹션에서

      1. **[!UICONTROL Plan name]**(예: `Demo plan`)을(를) 입력하십시오. **[!UICONTROL Description]**(예: `Demo plan for Luma company`)을(를) 입력하십시오.
      1. **[!UICONTROL _에서&#x200B;**[!UICONTROL Model]**을(를) 선택하십시오. 옵션을 선택하십시오._.]**.
      1. ![LinkOut](/help/assets//icons/LinkOut.svg) **[!UICONTROL Create model]**&#x200B;을(를) 선택하여 계획 생성 내에서 직접 모델을 만들 수 있습니다. 브라우저에서 새 탭이 열리고 [모델](../models/overview.md) 인터페이스가 표시됩니다.

         ![계획 설정](/help/assets//plan-setup.png)

   1. **[!UICONTROL Budget]** 섹션에서:

      1. 날짜를 입력하거나 ![달력](/help/assets//icons/Calendar.svg)을 사용하여 날짜 범위를 선택하여 날짜 범위를 지정하십시오.
      1. 예산을 입력합니다.

      각각 예산이 있는 날짜 범위를 추가하려면 ![CalendarAdd](/help/assets//icons/CalendarAdd.svg) **[!UICONTROL Add row]**&#x200B;을(를) 선택하십시오.

      날짜 범위 및 관련 예산을 삭제하려면 ![닫기](/help/assets//icons/Close.svg)를 선택하세요.

      지정된 최대 예산을 정의하려면

      1. **[!UICONTROL Maximize budget]** 스위치를 켭니다.
      1. 최대 예산 금액을 지정합니다. 금액은 날짜 범위에 대해 지정된 총 예산 금액보다 크거나 같아야 합니다.

         ![계획 예산](/help/assets//plan-budget.png)

   1. **[!UICONTROL Next]**&#x200B;를 선택합니다.

1. **[!UICONTROL Done with all required fields]** 대화 상자에서:

   ![계획 완료](/help/assets//plan-done-required-fields.png)

   * 선택 <img src="/help/assets//icons/NewPlan.svg" width="25" /> ROI가 예측되는 AI 추천 플랜을 생성하려면 **[!UICONTROL Create plan now]**&#x200B;을(를) 수행하십시오.

     **[!UICONTROL OK]**&#x200B;을(를) 선택합니다. 플랜이 생성되었습니다.


   * 예측된 ROI로 계획을 만들기 전에 채널 예산을 편집하려면 ![테이블 편집](/help/assets//icons/TableEdit.svg) **[!UICONTROL Edit channel budgets first]**&#x200B;을(를) 선택하십시오.

     다음 단계에서 **[!UICONTROL Spend selection]**&#x200B;에서 채널 지출을 정의할 수 있도록 **[!UICONTROL OK]**&#x200B;을(를) 선택하십시오.



1. **[!UICONTROL Spend selection]** 섹션에서 각 예산 날짜 범위에 대해 ![V자형 화살표](/help/assets//icons/ChevronRight.svg)를 사용하여 해당 데이터 범위에 대한 채널 배포 보기를 엽니다.

   1. 각 채널의 예산을 정의하려면 **[!UICONTROL Min]** 및 **[!UICONTROL Max]**&#x200B;의 값을 입력하거나 슬라이더를 사용하십시오.

   1. 통화 또는 백분율 입력 간을 전환하려면 **[!UICONTROL View spend by]**&#x200B;에 대해 **[!UICONTROL $]** 또는 **[!UICONTROL %]**&#x200B;을(를) 선택하세요.

      ![선택 비용](/help/assets//plan-spend-selection.png)

   1. 완료되면 **[!UICONTROL Create]**&#x200B;을(를) 선택합니다.

   1. **[!UICONTROL Create plan]** 대화 상자에서 **[!UICONTROL Create plan]**&#x200B;을(를) 선택하여 계획을 만듭니다. **[!UICONTROL Cancel]**&#x200B;을(를) 선택하여 플랜 만들기를 취소하세요. 확인을 위해 **[!UICONTROL No work is saved]** 대화 상자가 표시됩니다.
