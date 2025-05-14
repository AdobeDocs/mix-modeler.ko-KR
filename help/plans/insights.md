---
title: 플랜 인사이트
description: Mix Modeler에서 플랜에 대한 통찰력을 보고 플랜을 편집하는 방법을 알아봅니다.
feature: Plans
exl-id: 91385595-284f-4fcb-b54b-9539905e552b
source-git-commit: 3545a7045478108db4d9f6bb87df679bfede5a45
workflow-type: tm+mt
source-wordcount: '766'
ht-degree: 0%

---

# 플랜 인사이트


[!UICONTROL Plan insights]에서 플랜의 기반이 되는 [!UICONTROL Model], [!UICONTROL Data range] 및 [!UICONTROL Total budget]을(를) 표시하는 플랜 인사이트가 만들어집니다.

검색을 마치면 다음으로 구성된 계획의 개요가 표시됩니다.

- [!UICONTROL Forecasted paid channel ROI] 시각화
- [!UICONTROL Forecasted revenue] 시각화
- [!UICONTROL Forecasted conversion] 시각화
- [!UICONTROL Marginal channel return] 시각화
- 플랜의 [!UICONTROL Data range breakdown] 테이블, 열 표시

   - 채널
   - ROI
   - CPA
   - 매출
   - 전환 목표
   - 지출

인터페이스를 닫으려면 **[!UICONTROL Close]**&#x200B;을(를) 선택합니다.

플랜의 ROI를 보는 방법을 변경하려면 **[!UICONTROL X]** 또는 **[!UICONTROL  %]**(**[!UICONTROL View ROI]**)을(를) 선택하십시오.

## 유료 채널 지출 및 ROI 예측

이 시각화는 모델, 날짜 범위 및 예산을 기반으로 유료 채널의 예상 지출 및 투자 수익률에 대한 산포도를 보여 줍니다.

![유료 채널 지출 예측 및 ROI 시각화](../assets/overview-plan-forecasted-paid-channel-send-roi.png)


## 예상 수익

이 막대 차트 시각화는 모델, 날짜 범위 및 예산을 기반으로 채널에 대해 예측된 매출을 보여줍니다.

![예측된 매출 시각화](../assets/overview-plan-forecasted-revenue.png)


## 예측 전환

이 막대 차트 시각화는 모델, 날짜 범위 및 예산을 기반으로 채널에 대해 예측된 전환을 보여줍니다.

![예측된 전환 시각화](../assets/overview-plan-forecasted-conversions.png)


## 한계 채널 수익

이 선 차트 시각화는 **[!UICONTROL Marginal break-even]** 및 **[!UICONTROL Return point]**&#x200B;에 대한 지표가 있는 선택한 채널에 대한 한계 수익률 곡선을 보여 줍니다. 이 시각화를 통해 한계 손익분기점에 도달하여 채널에 대한 지출이 어떻게 되는지 그리고 채널 지출을 증가시킬 공간이 있는지 또는 채널 지출 효율성을 개선하기 위해 채널에 대한 지출을 줄여야 하는지 여부를 이해할 수 있습니다.

![한계 채널 반환 시각화](../assets/overview-plan-marginal-channel-return.png)

시각화에 사용할 특정 채널을 선택하려면 **[!UICONTROL View]** 드롭다운 메뉴에서 채널을 선택합니다.


## 날짜 범위 분류

[!UICONTROL Date range breakdown] 테이블은 [!UICONTROL ROI], [!UICONTROL Revenue], [!UICONTROL CPA], [!UICONTROL Conversions] 및 [!UICONTROL Spend]에 대한 채널별 세부 데이터를 보여줍니다.

![날짜 범위 분류 테이블](../assets/overview-plan-date-range-breakdown.png)

1. 날짜 범위 분류의 데이터가 포함된 CSV 파일을 다운로드하려면 ![다운로드](/help/assets/icons/Download.svg) **[!UICONTROL Download CSV]**&#x200B;을(를) 선택하십시오. 컨텍스트 메뉴에서:

   - CSV 형식의 자세한 데이터를 보려면 ![다운로드](/help/assets/icons/Download.svg) **[!UICONTROL Detailed CSV]**&#x200B;을(를) 선택하십시오.
   - CSV 형식의 요약 데이터를 보려면 ![다운로드](/help/assets/icons/Download.svg) **[!UICONTROL Summary CSV]**&#x200B;을(를) 선택하십시오.

   세부 데이터는 주별로 입력된 세부 데이터입니다. 요약 데이터는 모델이 제공한 날짜 범위에 의해 입력된 데이터입니다.

1. 채널의 범주별 날짜 범위 분류를 보려면 **[!UICONTROL View]** 선택에서 **[!UICONTROL All channels]**, **[!UICONTROL Paid channels]** 또는 **[!UICONTROL Non-paid channels]**&#x200B;을(를) 선택하십시오.


## 플랜 편집

1. 플랜을 편집하려면 ![편집](/help/assets/icons/Edit.svg) **[!UICONTROL Edit plan]**&#x200B;을(를) 선택하십시오.

   1. **[!UICONTROL Spend selection]** 섹션에서 각 예산 날짜 범위에 대해 ![V자형 화살표](/help/assets/icons/ChevronRight.svg)를 사용하여 해당 데이터 범위에 대한 채널 배포 보기를 엽니다.

   1. 각 채널의 예산을 수정하려면 **[!UICONTROL Min]** 및 **[!UICONTROL Max]**&#x200B;의 값을 수정하거나 슬라이더를 사용하십시오.

   1. 통화 또는 백분율 입력 간을 전환하려면 **[!UICONTROL View spend by]**&#x200B;에 대해 **[!UICONTROL $]** 또는 **[!UICONTROL %]**&#x200B;을(를) 선택하세요.

      ![선택 비용](/help/assets/spend-selection.png)

   1. 플랜 세부 정보를 편집하려면 **[!UICONTROL Edit details]**&#x200B;을(를) 선택하세요.

      1. **[!UICONTROL Setup]** 섹션에서 해당되는 경우 **[!UICONTROL Plan name]** 및 **[!UICONTROL Description]**&#x200B;을(를) 수정합니다.

      1. **[!UICONTROL Budget]** 섹션에서:

         1. 날짜를 입력하거나 ![달력](/help/assets/icons/Calendar.svg)을 사용하여 날짜 범위를 선택하여 하나 이상의 플랜 날짜 범위에 대한 **[!UICONTROL Date range]**&#x200B;을(를) 수정합니다.

         1. 플랜의 날짜 범위 중 하나 이상에 대한 **[!UICONTROL Budget]**&#x200B;을(를) 수정합니다.

         각각 예산이 있는 날짜 범위를 추가하려면 ![CalendarAdd](/help/assets/icons/CalendarAdd.svg) **[!UICONTROL Add row]**&#x200B;을(를) 선택하십시오.

         날짜 범위 및 관련 예산을 삭제하려면 ![닫기](/help/assets/icons/Close.svg)를 선택하세요.

         최대 예산을 정의하려면

         1. **[!UICONTROL Maximize budget]** 스위치를 켭니다.
         1. 최대 예산 금액을 지정합니다. 금액은 날짜 범위에 대해 지정된 총 예산 금액보다 크거나 같아야 합니다.

      1. **[!UICONTROL Spend]** 섹션으로 돌아가려면 **[!UICONTROL Next]**&#x200B;을(를) 선택하십시오. 플랜 개요로 돌아가려면 **[!UICONTROL Cancel]**&#x200B;을(를) 선택하세요.

         ![플랜 세부 정보](/help/assets/plan-details.png)

   1. 플랜에 대한 고급 구성을 정의한 경우 **[!UICONTROL Next]**&#x200B;을(를) 선택합니다.

      ![고급 구성 편집](../assets/edit-plan-advanced-configuration.png)

      - 계획명 , 모델, 날짜 범위 및 총 예산이 요약됩니다.

      - 기본적으로 Mix Modeler은 최신 이전 시즌 데이터를 사용하여 전환당 평균 매출을 자동으로 계산합니다. **[!UICONTROL Average Revenue per conversion]**&#x200B;에서 전환당 특정 평균 매출을 정의할 수 있습니다.

         1. 예산의 각 일자 범위에 대해
            1. **[!UICONTROL Date range]** 드롭다운 메뉴에서 날짜 범위를 선택합니다.
            1. **[!UICONTROL Average revenue]** 값을 입력하십시오.

         1. ![AddCircle](/help/assets/icons/AddCircle.svg) 전환 단위당 사용자 지정 평균 수익 추가를 선택하여 날짜 범위를 추가합니다.
         1. 날짜 범위를 제거하려면 ![RemoveCircle](/help/assets/icons/RemoveCircle.svg)을(를) 선택하십시오.

        >[!NOTE]
        >
        >모델에 이전 수익 데이터가 포함되지 않은 경우 예산에 대해 지정한 각 날짜 범위에 대해 전환당 평균 수익을 정의해야 합니다.
        >

      - 기본적으로 Mix Modeler은 최신 시즌 데이터를 사용하여 채널 비용을 자동으로 계산합니다. **[!UICONTROL Channel costs]**&#x200B;에서 사용자 지정 채널 비용을 정의할 수 있습니다.

         1. 모델의 각 채널에 대해 사용자 지정 채널 비용을 정의합니다.
            1. **[!UICONTROL Channel]** 드롭다운 메뉴에서 채널을 선택합니다.
            1. 예산의 각 일자 범위에 대해
               1. **[!UICONTROL Date range]** 드롭다운 메뉴에서 날짜 범위를 선택합니다.
               1. **[!UICONTROL Average revenue]** 값을 입력하십시오.
            1. 날짜 범위를 추가하려면 ![AddCircle](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add custom average revenue per conversion unit]**&#x200B;을(를) 선택하십시오.
            1. 날짜 범위를 제거하려면 ![RemoveCircle](/help/assets/icons/RemoveCircle.svg)을(를) 선택하십시오.

         1. 채널을 추가하려면 ![AddCircle](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add custom channel cost]**&#x200B;을(를) 선택하십시오.
         1. 사용자 지정 채널을 제거하려면 ![CrossSize400](/help/assets/icons/CrossSize400.svg)을(를) 선택하십시오.


1. 플랜 편집이 완료되면 **[!UICONTROL Edit]**&#x200B;을(를) 선택하세요.

   **[!UICONTROL All changes are final]** 대화 상자에서 **[!UICONTROL OK]**&#x200B;을(를) 선택하여 플랜의 현재 지출 할당과 ROI 및 매출 예측을 업데이트합니다. 플랜 업데이트를 취소하려면 **[!UICONTROL Cancel]**&#x200B;을(를) 선택하세요.

1. 플랜 업데이트를 취소하려면 **[!UICONTROL Cancel]**&#x200B;을(를) 선택하세요.

   **[!UICONTROL No work will be saved]** 대화 상자에서 **[!UICONTROL Cancel]**&#x200B;을(를) 선택하여 플랜 작업을 계속하거나 **[!UICONTROL OK]**&#x200B;을(를) 선택하여 플랜 인터페이스로 돌아갑니다.
