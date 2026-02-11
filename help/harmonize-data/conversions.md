---
title: 전환
description: Mix Modeler에서 데이터를 조화롭게 만드는 과정의 일부로 사용할 전환을 만드는 방법을 알아봅니다.
feature: Harmonized Data, Conversions
exl-id: a8559426-452a-43e8-9a60-0c0bc97d863c
source-git-commit: 5468e0aaf37bf2dca8912199ea26e5f8d9069cb5
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 2%

---

# 전환 {#conversions}


>[!CONTEXTUALHELP]
>id="harmonizeddata_conversions_create"
>title="전환"
>abstract="전환 이벤트는 마케팅 활동의 영향을 식별하는 비즈니스 목표입니다. 예: 전자 상거래 주문, 매장 내 구매, 웹 사이트 방문 등."


전환 이벤트는 마케팅 활동의 영향을 식별하는 비즈니스 목표입니다. 예: 전자 상거래 주문, 매장 내 구매, 웹 사이트 방문 등.

속성 분석을 위한 마케팅 전환을 정의합니다.

## 전환 관리

Mix Modeler 인터페이스에서 사용 가능한 전환의 표를 보려면 다음을 수행하십시오.

1. 왼쪽 레일에서 ![DataSearch](/help/assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]**&#x200B;을(를) 선택합니다.

1. 상단 표시줄에서 **[!UICONTROL Conversions]**&#x200B;을(를) 선택합니다. 전환 테이블이 표시됩니다.

테이블 열은 변환에 대한 세부 사항을 지정합니다.

| 열 이름 | 세부 사항 |
| --- | ---|
| 이름 | 전환의 이름입니다. |
| 수입 | 전환으로 인한 매출을 계산하는 데 사용할 조정된 데이터 지표입니다. |
| 전환 지표 | 분석을 위한 전환 지표로 사용할 조정된 데이터 지표입니다. |
| 카테고리 | 전환의 전환 카테고리입니다. |
| 생성됨 | 변환 생성 날짜 및 시간입니다. |
| 마지막 수정일 | 전환을 마지막으로 수정한 날짜 및 시간입니다. |


## 전환 추가

전환을 추가하려면 Mix Modeler의 ![DataSearch](/help/assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Conversion]** 인터페이스에서 다음을 수행합니다.

1. ![추가](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add a conversion]**&#x200B;을(를) 선택합니다.

1. **[!UICONTROL Create conversion]** 대화 상자에서:

   1. **[!UICONTROL Conversion]**&#x200B;의 이름을 입력하십시오(예: `Store Conversions`).

   1. **[!UICONTROL Conversion category]** 정의.

      1. **[!UICONTROL *조화를 선택하십시오...*]**(예: `Conversion types`)에서 값을 선택하십시오.

      1. 연산자 ![V자형 화살표](/help/assets/icons/ChevronDown.svg)의 값을 선택하십시오(예: **[!UICONTROL is]**).

      1. **[!UICONTROL *값 선택&#x200B;*]**에서 값을 선택하거나&#x200B;**[!UICONTROL Store]**과(와) 같은 값을 입력하십시오.

   1. **[!UICONTROL Conversion metric for analysis]**&#x200B;에서 조정된 필드를 선택합니다(예: **[!UICONTROL Orders]**).

   1. **[!UICONTROL Revenue field]**&#x200B;에서 조정된 필드를 선택합니다(예: **[!UICONTROL Gross Demand]**).

   1. 변환을 만들려면 **[!UICONTROL Create]**&#x200B;을(를) 선택합니다. 전환 만들기를 취소하려면 **[!UICONTROL Cancel]**&#x200B;을(를) 선택합니다.

      ![대체 텍스트](/help/assets/create-conversion.png)

1. 이 필드를 만들면 전환 표에 전환이 추가됩니다.


## 세부 정보 보기

변환의 세부 사항을 보려면 다음과 같이 하십시오.

1. 테이블의 전환 이름 위로 마우스를 가져가면 ![자세히](/help/assets/icons/More.svg)를 선택합니다.

1. ![보기](/help/assets/icons/ViewDetail.svg) **세부 정보 보기**&#x200B;를 선택합니다. 대화 상자에 전환에 대한 세부 정보가 표시됩니다. 자세한 내용은 [전환 추가](#add-a-conversion)를 참조하십시오. 대화 상자를 닫으려면 **[!UICONTROL Cancel]**&#x200B;을(를) 선택하십시오.

## 보고서 보기

전환 보고서를 보려면 다음 작업을 수행하십시오.

1. 테이블의 전환 이름 위로 마우스를 가져가면 ![자세히](/help/assets/icons/More.svg)를 선택합니다.

1. ![GraphTrend](/help/assets/icons/GraphTrend.svg) **보고서 보기**&#x200B;를 선택합니다. 대화 상자에 전환 보고서가 표시됩니다.

   ![전환 보기 보고서](../assets/conversion-view-report.png)

   * 보고할 세부 기간을 변경하려면 **[!UICONTROL Weekly]** 드롭다운 메뉴에서 값을 선택합니다.
   * 보고할 기간을 변경하려면 시작 및 종료 날짜를 입력하거나 ![달력](/help/assets/icons/Calendar.svg)을 사용하여 달력 팝업에서 기간을 정의하십시오.

1. 대화 상자를 닫으려면 **[!UICONTROL Close]**&#x200B;을(를) 선택하십시오.

## 전환 삭제

변환을 삭제하려면 다음 작업을 수행하십시오.

1. 테이블의 전환 이름 위로 마우스를 가져갈 때 ![삭제](/help/assets/icons/Delete.svg) **삭제**&#x200B;를 선택합니다.
1. **[!UICONTROL Delete conversion]** 대화 상자 확인 대화 상자에서 **[!UICONTROL Delete]**&#x200B;을(를) 선택하여 전환을 영구적으로 삭제합니다.
