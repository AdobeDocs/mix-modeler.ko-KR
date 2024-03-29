---
title: 전환
description: Mix Modeler에서 데이터를 조화시키는 과정에서 사용할 전환을 만드는 방법을 알아봅니다.
feature: Harmonized Data, Conversions
exl-id: a8559426-452a-43e8-9a60-0c0bc97d863c
source-git-commit: 86732fe30637aa72ced232d9f331a3cc64baa39b
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 1%

---

# 전환

전환 이벤트는 마케팅 활동의 영향을 식별하는 비즈니스 목표입니다. 예: 전자 상거래 주문, 매장 내 구매, 웹 사이트 방문 등.

속성 분석을 위한 마케팅 전환을 정의합니다.

## 전환 관리

Mix Modeler 인터페이스에서 사용 가능한 전환의 표를 보려면 다음을 수행하십시오.

1. 선택 ![데이터 검색](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** 왼쪽 레일에서.

1. 선택 **[!UICONTROL Conversions]** 을 클릭합니다. 전환 테이블이 표시됩니다.

테이블 열은 변환에 대한 세부 사항을 지정합니다.

| 열 이름 | 세부 사항 |
| --- | ---|
| 이름 | 전환의 이름입니다. |
| 매출 | 전환으로 인한 매출을 계산하는 데 사용할 조정된 데이터 지표입니다. |
| 전환 지표 | 분석을 위한 전환 지표로 사용할 조정된 데이터 지표입니다. |
| 카테고리 | 전환의 전환 카테고리입니다. |
| 생성됨 | 변환 생성 날짜 및 시간입니다. |
| 마지막 수정일 | 전환을 마지막으로 수정한 날짜 및 시간입니다. |

{style="table-layout:auto"}

## 전환 추가

변환을 추가하려면 ![데이터 검색](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Conversion]** Mix Modeler 인터페이스:

1. 선택 ![추가](../assets/icons/AddCircle.svg) **[!UICONTROL Add a conversion]**.

1. 다음에서 **[!UICONTROL Create conversion]** 대화 상자:

   1. 이름 입력 **[!UICONTROL Conversion]**, 예 `Store Conversions`.

   1. 다음을 정의합니다. **[!UICONTROL Conversion category]**.

      1. 다음에서 값 선택 **[!UICONTROL *조화 선택...*]**, 예 `Conversion types`.

      1. 연산자 값 선택 ![펼침](../assets/icons/ChevronDown.svg), 예 **[!UICONTROL is]**.

      1. 다음에서 값 선택 **[!UICONTROL *값 선택&#x200B;*]**또는 값을 입력합니다(예: ).**[!UICONTROL Store]**.

   1. 다음 위치에서 조화로운 필드 선택 **[!UICONTROL Conversion metric for analysis]**, 예 **[!UICONTROL Orders]**.

   1. 다음 위치에서 조화로운 필드 선택 **[!UICONTROL Revenue field]**, 예 **[!UICONTROL Gross Demand]**.

   1. 변환을 만들려면 다음을 선택합니다. **[!UICONTROL Create]**. 변환 생성을 취소하려면 **[!UICONTROL Cancel]**.

      ![대체 텍스트](../assets/create-conversion.png)

1. 이 필드를 만들면 전환 표에 전환이 추가됩니다.


## 전환 보기

전환을 보려면 다음 작업을 수행하십시오.

1. 선택 ![자세히](../assets/icons/More.svg) 마우스로 테이블의 전환 이름을 가리키면

1. 선택 ![보기](../assets/icons/ViewDetail.svg) **보기**. 대화 상자에 전환에 대한 세부 정보가 표시됩니다. 다음을 참조하십시오 [전환 추가](#add-a-conversion) 추가 정보. 선택 **[!UICONTROL Cancel]** 대화 상자를 닫습니다.


## 전환 삭제

변환을 삭제하려면 다음 작업을 수행하십시오.

1. 선택 ![삭제](../assets/icons/Delete.svg) **삭제** 마우스로 테이블의 전환 이름을 가리키면
1. 다음에서 **[!UICONTROL Delete conversion]** 대화 상자 확인 대화 상자 선택 **[!UICONTROL Delete]** 변환 삭제.
