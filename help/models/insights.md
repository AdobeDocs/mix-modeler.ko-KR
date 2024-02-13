---
title: 모델 인사이트
description: Mix Modeler 시 기록 개요, 모델 통찰력 및 모델 품질과 같은 모델에 대한 세부 정보를 얻는 방법에 대해 알아봅니다.
feature: Models
exl-id: d99852f9-ba0d-4a2e-b5f3-ca0efe6002fd
source-git-commit: 17d4609f251808f68372185ac90530e164024b5f
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---

# 모델 인사이트

모델 인사이트를 보려면 ![모델](../assets/icons/FileData.svg) **[!UICONTROL Models]** Mix Modeler 인터페이스:

1. 을(를) 가진 모델 이름 선택 **[!UICONTROL Last run status]** / <span style="color:green">●</span> **[!UICONTROL Success]** 다음에서 **[!UICONTROL Models]** 테이블.

1. 컨텍스트 메뉴에서 을(를) 선택합니다 **[!UICONTROL Model Insights]**.

내역 개요, 모델 인사이트 및 모델 품질의 세 가지 탭을 사용하여 지정된 모델이 마지막으로 새로 고쳐지고 위젯이 표시되는 것을 볼 수 있습니다.

각 탭의 위젯이 기반으로 하는 날짜 기간을 변경할 수 있습니다. 날짜 기간을 입력하거나 선택 ![캘린더](../assets/icons/Calendar.svg) 날짜 기간을 선택합니다.


## 내역 개요

내역 개요 탭에는 다음에 대한 위젯이 표시됩니다.

* 회계 분기 및 제품별 전환 및 소비.

* 채널별 소비.

* 접점 사용.

  이 위젯에 대해 표시할 대체 지출 기반 채널을 선택할 수 있습니다. 다음 위치에서 채널 선택 **[!UICONTROL Channels]**.

* 접점 볼륨.

  이 위젯에 대해 표시할 대체 볼륨 기반 채널을 선택할 수 있습니다. 다음 위치에서 채널 선택 **[!UICONTROL Channels]**.

![모델 - 기록 개요](../assets/model-historical-overview.png)

## 모델 인사이트

모델 인사이트 탭에는 다음에 대한 위젯이 표시됩니다.

* 날짜 및 기본 미디어별 기여도. 누적 그래프는 맨 아래에 기준, 중간에 비 지출 채널 및 맨 위에 지출 채널의 순서로 정렬됩니다.

* 채널별 기여도.

* 마케팅 성과 요약.

* 한계 응답 곡선.

![모델 - 모델 인사이트](../assets/model-model-insights.png)

각 위젯의 개별 차트 요소 위로 마우스를 가져가면 자세한 내용과 함께 팝오버를 표시할 수 있습니다.

위젯에 대한 데이터가 포함된 CSV 파일을 다운로드하려면 을 선택합니다. ![다운로드](../assets/icons/Download.svg).

Microsoft® Excel 형식으로 전체 모델 통찰력 데이터를 다운로드하려면 다음을 선택합니다. ![다운로드](../assets/icons/Download.svg) **[!UICONTROL Download data]**.




## 모델 품질

모델 품질 탭에는 측정을 위한 위젯이 표시됩니다.

* 자료가 회귀 모형(적합도)에 얼마나 잘 부합하는지를 알려주는 R2(R-제곱)이다.

* MAPE(Mean Absolute Percentage Error): 예측 정확도를 측정하기 위해 가장 일반적으로 사용되는 KPI 중 하나이며 예측 오류를 실제 값의 백분율로 표시합니다.

* RMSE(제곱 평균 제곱근 오차): 오차의 제곱에 따라 가중치가 적용된 평균 &quot;오차&quot;를 표시합니다.

![모델 품질](../assets/model-quality.png)

위젯에 대한 데이터가 포함된 CSV 파일을 다운로드하려면 을 선택합니다. ![자세히](../assets/icons/More.svg) 위젯 및 컨텍스트 메뉴에서 ![다운로드](../assets/icons/Download.svg) **[!UICONTROL Download as CSV]**.
