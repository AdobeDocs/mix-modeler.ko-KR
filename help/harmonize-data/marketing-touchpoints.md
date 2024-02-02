---
title: 마케팅 접점
description: Mix Modeler에서 데이터를 조화롭게 만드는 과정의 일부로 사용할 마케팅 접점을 만드는 방법을 알아봅니다.
feature: Harmonized Data, Marketing Touch Points
exl-id: 42851107-7568-4bc9-92ca-3cba713a522e
source-git-commit: 86732fe30637aa72ced232d9f331a3cc64baa39b
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 0%

---

# 마케팅 접점

마케팅 접점은 마케팅 투자가 숫자 또는 수익 기반 전환에 미치는 영향을 평가하는 데 사용되는 수신자, 개인 및/또는 쿠키 수준 마케팅 이벤트입니다.

속성 분석을 지원하는 마케팅 접점을 정의합니다.

## 마케팅 접점 관리

Mix Modeler 인터페이스에서 사용 가능한 마케팅 접점 테이블을 보려면 다음을 수행하십시오.

1. 선택 ![데이터 검색](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** 왼쪽 레일에서.

1. 선택 **[!UICONTROL Marketing touchpoint]** 을 클릭합니다. 마케팅 접점 테이블이 표시됩니다. 사용 가능한 페이지가 더 있으면 다음을 사용합니다. ![왼쪽 화살표](../assets/icons/ChevronLeft.svg) 또는 ![오른쪽 화살표](../assets/icons/ChevronRight.svg) 위치: **[!UICONTROL Page _x _/_x_]** 을 눌러 테이블의 페이지 사이를 이동합니다.

테이블 열은 마케팅 접점에 대한 세부 사항을 지정합니다.

| 열 이름 | 세부 사항 |
| --- | ---|
| 이름 | 마케팅 접점 이름입니다. |
| 지출 지표 | 접점 지출을 계산하는 데 사용할 조정된 데이터 지표입니다. |
| 볼륨 지표 | 접점 볼륨을 계산하는 데 사용할 조정된 데이터 지표입니다. |
| 규칙 | 사용할 터치포인트 규칙입니다. |
| 생성됨 | 마케팅 접점 생성 날짜 및 시간입니다. |
| 마지막 수정일 | 마케팅 접점을 마지막으로 수정한 날짜 및 시간입니다. |

{style="table-layout:auto"}

## 마케팅 접점 추가

마케팅 접점을 추가하려면 ![데이터 검색](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Marketing touchpoint]** Mix Modeler 인터페이스:

1. 선택 ![추가](../assets/icons/AddCircle.svg) 마케팅 접점 추가.

1. 다음에서 **[!UICONTROL Marketing touchpoint]** 대화 상자.

   1. 이름 입력 **[!UICONTROL Touchpoint Name]**, 예 `Luma Touchpoint`.

   1. 정의 **[!UICONTROL Touchpoint rule]**.

      1. 다음에서 값 선택 **[!UICONTROL *조화됨 선택&#x200B;*]**, 예&#x200B;**[!UICONTROL Brand]**.

      1. 연산자 값 선택 ![펼침](../assets/icons/ChevronDown.svg), 예 **[!UICONTROL is]**.

      1. 다음에서 값 선택 **[!UICONTROL *값 선택&#x200B;*]**또는 값을 입력합니다(예: ).**[!DNL Luma]**.

   1. 다음 위치에서 조화로운 필드 선택 **[!UICONTROL Touchpoint volume]**, 예 **[!UICONTROL Impressions]**.

   1. 다음 위치에서 조화로운 필드 선택 **[!UICONTROL Touchpoint spend]**, 예 **[!UICONTROL Cost]**.

      ![마케팅 접점](../assets/create-touchpoint.png)

   1. 마케팅 접점을 만들려면 다음을 선택합니다. **[!UICONTROL Create]**. 마케팅 접점 만들기를 취소하려면 **[!UICONTROL Cancel]** .

1. 터치포인트를 만들면 마케팅 터치포인트 테이블에 터치포인트가 추가됩니다.


## 마케팅 접점 보기

마케팅 접점을 보려면 다음을 수행하십시오.

1. 선택 ![자세히](../assets/icons/More.svg) 마우스로 테이블의 마케팅 접점 이름을 가리키면,

1. 선택 ![보기](../assets/icons/ViewDetail.svg) **보기**. 대화 상자에 마케팅 접점의 세부 정보가 표시됩니다. 다음을 참조하십시오 [마케팅 접점 추가](#add-a-marketing-touchpoint) 추가 정보. 선택 **[!UICONTROL Cancel]** 대화 상자를 닫습니다.


## 마케팅 접점 삭제

마케팅 접점 삭제 방법:

1. 선택 ![삭제](../assets/icons/Delete.svg) **삭제** 마우스로 테이블의 마케팅 접점 이름을 가리키면,
1. 다음에서 **[!UICONTROL Delete touchpoint]** 대화 상자 확인 대화 상자 선택 **[!UICONTROL Delete]** 마케팅 접점 을 영구적으로 삭제합니다.

