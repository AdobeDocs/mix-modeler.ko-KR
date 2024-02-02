---
title: Harmonized data overview 대시보드
description: Mix Modeler에서 Harmonized Data Overview 대시보드를 사용하는 방법에 대해 알아봅니다.
feature: Dashboard, Harmonized Data
exl-id: fbb01613-d648-4db1-a782-a7720b7a03ad
source-git-commit: 86732fe30637aa72ced232d9f331a3cc64baa39b
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# Harmonized data 개요

Mix Modeler 개요의 통합 데이터 탭은 수집된 데이터 및 통합 데이터 설정의 일부로 사용하도록 구성한 통합 데이터에 대한 통찰력을 제공합니다.

개요는 4개의 KPI 상태 카드 위젯(상단 행)과 6개의 다른 구성 가능한 위젯을 보여 줍니다.

위젯에 표시할 데이터의 날짜 기간을 변경하려면 시작 날짜 및 종료 날짜를 수동으로 입력하거나 다음을 사용하여 기간을 선택합니다. ![캘린더](../assets/icons/Calendar.svg).

## 데이터 필터

를 사용하여 모든 위젯에 대해 표시되는 데이터를 필터링할 수 있습니다. ![필터](../assets/icons/Filter.svg) **[!UICONTROL Category Filters]** 창.

각 카테고리에 대해 하나 이상의 필터를 선택합니다(**[!UICONTROL Brands]**, **[!UICONTROL Campaigns]**, **[!UICONTROL Cannels Type]**, **[!UICONTROL Conversion types]**, **[!UICONTROL Datasets]**, **[!UICONTROL Media types]**, **[!UICONTROL Source types]**, 및 **[!UICONTROL Traffic Source]**).

선택한 필터는 다음 위젯의 맨 위에 표시됩니다. **[!UICONTROL FILTERING BY:]**.

1. 개별 필터를 제거하려면 다음을 선택합니다 ![닫기](../assets/icons/Close.svg) 다음 위치에 나열된 필터에서 **[!UICONTROL FILTERING BY:]**.

1. 다음을 사용하여 모든 필터를 빠르게 지울 수 있습니다. **[!UICONTROL Clear All]**.

![Harmonized data 개요](../assets/harmonized-data-overview.png)


## 위젯 구성

각 위젯을 구성할 수 있습니다.

* KPI 상태 카드 위젯에서:

   1. 선택 ![편집](../assets/icons/Edit.svg) 및 ![편집](../assets/icons/Edit.svg) **[!UICONTROL Edit data]** 컨텍스트 메뉴 아래의 제품에서 사용할 수 있습니다.

   1. 다음에서 **[!UICONTROL KPI status card]** 대화 상자:

      1. 선택 **[!UICONTROL KPI]** 목록에서 삭제할 수 있습니다.

      1. 선택 **[!UICONTROL Apply]** 카드에 변경 사항을 적용합니다. 선택 **[!UICONTROL Cancel]** 변경을 취소합니다.

* 기타 구성 가능한 위젯의 경우:

   1. 선택 ![편집](../assets/icons/Edit.svg) 및 ![편집](../assets/icons/Edit.svg) **[!UICONTROL Edit data]** 컨텍스트 메뉴 아래의 제품에서 사용할 수 있습니다.

   1. 다음에서 **[!UICONTROL Edit Data]** 대화 상자:

      1. 다음에서 지표 선택 **[!UICONTROL Select a metric]**, 예 **[!UICONTROL Impressions]**.
      1. 다음에서 범주 선택 **[!UICONTROL Select category]**, 예 **[!UICONTROL Media types]**.
      1. (선택 사항) 다음 중에서 두 번째 범주를 선택합니다. **[!UICONTROL Select second category (optional)]**, 예 **[!UICONTROL Traffic sources]**.
      1. 선택 ![시계](../assets/icons/Clock.svg) **[!UICONTROL Time]** 또는 ![계산기](../assets/icons/Calculator.svg) **[!UICONTROL Total]** 의 분석 유형으로 **[!UICONTROL Select analysis type]**.

         다음을 선택하는 경우 ![시계](../assets/icons/Clock.svg) **[!UICONTROL Time]**&#x200B;시간 빈도를 지정할 수 있습니다. 선택 **[!UICONTROL Daily]**, **[!UICONTROL Weekly]**, **[!UICONTROL Monthly]** 또는 **[!UICONTROL Quarterly]** 출처: **[!UICONTROL Select time frequency]**.

         에서 현재 선택 항목의 업데이트된 미리보기를 볼 수 있습니다. [!UICONTROL Preview Area] 및 아래에 있는 현재 위젯 [!UICONTROL Current].

         ![통합 데이터 위젯 편집](../assets/edit-harmonized-data-widget.png)

         데이터를 사용할 수 없어 미리보기를 렌더링할 수 없는 경우 ![데이터 오류](../assets/icons/DataUnavailable.svg) [!UICONTROL Insights Not Available] - [!UICONTROL Harmonized fields are not available].

      1. 선택 **[!UICONTROL Apply]** 위젯에 변경 내용을 적용합니다. 선택 **[!UICONTROL Cancel]** 를 클릭하여 현재 위젯에 대한 모든 변경 사항을 취소합니다.
