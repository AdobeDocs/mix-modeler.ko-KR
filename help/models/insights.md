---
title: 모델 인사이트
description: Mix Modeler 시 기록 개요, 모델 통찰력 및 모델 품질과 같은 모델에 대한 세부 정보를 얻는 방법에 대해 알아봅니다.
feature: Models
exl-id: d99852f9-ba0d-4a2e-b5f3-ca0efe6002fd
source-git-commit: b503abc710bf3688c1b8219ddd2d242932916501
workflow-type: tm+mt
source-wordcount: '1159'
ht-degree: 0%

---

# 모델 인사이트

모델 인사이트를 보려면 ![모델](../assets/icons/FileData.svg) **[!UICONTROL Models]** Mix Modeler 인터페이스:

1. 다음에서 **[!UICONTROL Models]** 테이블에서 **[!UICONTROL Last run status]** / <span style="color:green">●</span> **[!UICONTROL Success]**.

1. 컨텍스트 메뉴에서 을(를) 선택합니다 **[!UICONTROL Model Insights]**.

![모델 인사이트 탭 막대](../assets/model-insights-tabbar.png)

지정된 모델이 마지막으로 새로 고쳐지고 위젯이 다음 네 가지 탭을 사용하여 표시되는 것을 볼 수 있습니다. [모델 인사이트](#model-insights), [속성](#attribution), [진단](#diagnostics), 및 [내역 개요](#historical-overview).

각 탭의 위젯이 기반으로 하는 날짜 기간을 변경할 수 있습니다. 날짜 기간을 입력하거나 선택 ![캘린더](../assets/icons/Calendar.svg) 날짜 기간을 선택합니다.

## [!UICONTROL Model insights]

모델 인사이트 탭에는 다음에 대한 위젯이 표시됩니다.

* 날짜 및 기본 미디어별 기여도. 누적 그래프는 맨 아래에 기준, 중간에 비지출 채널 및 맨 위에 지출 채널의 순서로 정렬됩니다.

* 채널별 기여도.

* 마케팅 성과 요약.

* 한계 응답 곡선.
  <br/>에서 채널 선택 **[!UICONTROL Channel]** 드롭다운 목록을 사용하여 특정 채널에 대한 위젯을 업데이트합니다.

![모델 - 모델 인사이트](../assets/model-insights-insights.png)

각 위젯의 개별 차트 요소 위로 마우스를 가져가면 자세한 내용과 함께 팝오버를 표시할 수 있습니다.

위젯에 대한 데이터가 포함된 CSV 파일을 다운로드하려면 을 선택합니다. ![다운로드](../assets/icons/Download.svg).

Microsoft® Excel 형식으로 전체 모델 통찰력 데이터를 다운로드하려면 다음을 선택합니다. ![다운로드](../assets/icons/Download.svg) **[!UICONTROL Download data]**.

## [!UICONTROL Attribution]

사용 [!UICONTROL Attribution] 탭에서는 이벤트 수준 데이터가 있는 터치포인트 및 마케팅 캠페인의 효과를 이해할 수 있습니다. 지원되는 속성 모델은 다음과 같습니다.

* Mix Modeler에서 선택한 모델 기반:
   * 알고리즘 - 영향
   * 알고리즘 - 증분
* 규칙 기반:
   * 가치 감소 단위
   * 첫 번째 터치
   * 마지막 터치
   * 선형
   * U자형

다음을 참조하십시오 [다중 터치 속성](../get-started/about.md#multi-touch-attribution) Mix Modeler의 멀티 터치 속성 기능에 대한 소개.

에서 하나 이상의 속성 모델을 선택합니다. **[!UICONTROL Attribution Model]** 드롭다운 목록입니다. 선택한 속성 모델은 속성 탭의 모든 위젯에 적용됩니다.

![속성](../assets/model-insights-attribution.png)

Mix Modeler 멀티 터치 속성 세분화된 이벤트 점수는 전체 Mix Modeler 점수 및 ROI에 맞게 조정됩니다. 이러한 점수는 Experience Platform에서 데이터 세트로 사용할 수도 있습니다.

속성 탭은 다음 위젯으로 구성됩니다.

### [!UICONTROL Overview]

다음 [!UICONTROL Overview] 위젯은 선택한 속성 모델에 대한 전환 합계 및 백분율을 보여 줍니다. 모델을 더 선택하면 시각화에 범례에 해당하는 자체 색상이 있는 원이 더 추가됩니다.

속성 모델에 대한 세부 사항이 있는 팝업을 보려면 시각화의 원 위로 마우스를 가져갑니다.

### [!UICONTROL Trends]

다음 [!UICONTROL Daily trends], [!UICONTROL Weekly trends], 또는 [!UICONTROL Monthly trends] 위젯은 선택한 속성 모델에 대해 일별, 주별 또는 월별 전환 트렌드를 표시합니다.

기간을 선택하려면 다음을 선택합니다 **[!UICONTROL Daily trends]**, **[!UICONTROL Weekly trends]** 또는 **[!UICONTROL Monthly trends]** 출처: ![자세히](../assets/icons/More.svg).

세부 정보를 보려면 특정 속성 모델의 데이터 라인 위로 마우스를 가져가 해당 데이터에 대한 총 전환 수를 표시하는 팝오버를 표시합니다.

### [!UICONTROL Breakdown]

다음 [!UICONTROL Breakdown] 위젯은 선택한 각 속성 모델에 대한 전환의 채널 또는 터치 포인트별 분류입니다. 이 위젯은 각 채널 또는 터치포인트의 효과를 결정하는 데 도움이 될 수 있습니다.

분류 유형을 선택하려면 **[!UICONTROL Breakdown by channel]** 또는 **[!UICONTROL Breakdown by touchpoint]** 출처: ![자세히](../assets/icons/More.svg).

세부 정보를 보려면 차트 요소 위로 마우스를 가져갑니다.

### [!UICONTROL Top campaigns]

최상위 캠페인 위젯은 캠페인 이름, 채널, 미디어 유형 및 증분 전환에 대한 열이 있는 최상위 캠페인의 테이블을 표시합니다. 이 위젯은 주어진 채널에 대한 특정 캠페인의 효과를 팀에 알리고 추가로 투자해야 하는 캠페인에 대한 통찰력을 제공하는 데 도움이 될 수 있습니다.

채널, 미디어 유형 또↑ 증분 전환에 ↓ 오름차순 또는 내림차순으로 테이블을 정렬하려면 열 헤더를 선택하고 정렬을 토글합니다.

별도의 대화 상자에서 테이블을 확장하려면 다음을 선택합니다 **[!UICONTROL Expand]** 출처: ![자세히](../assets/icons/More.svg).

확장된 [상위 캠페인] 대화 상자에는 다음과 같은 추가 열이 있는 동일한 테이블이 표시됩니다.

* 증분 전환
* 영향을 받은 전환
* 첫 번째 터치 전환
* 마지막 터치 전환

  추가 열 헤더를 각각 선택하여 테이블을 오름차순 또는 내림차순으로 정렬할 수 있습니다.

확장된 [최상위 캠페인] 대화 상자를 닫으려면 다음을 선택합니다. **[!UICONTROL Close]**.


### [!UICONTROL Breakdown by touchpoint position]

다음 [!UICONTROL Breakdown by touchpoint position] 시각화는 모든 전환 경로에서 접점 및 접점 위치별 속성 전환의 분류입니다. 이 차트는 터치포인트가 나머지 위치와 다른 위치보다 한 위치에서 더 잘 기여하는지 비교하는 데 도움이 됩니다.

>[!NOTE]
>
>모든 접점 및 위치에서 속성 모델에 대한 백분율 기여도의 합계는 100이어야 합니다.


위치 [!UICONTROL Starter], [!UICONTROL Player] 및 [!UICONTROL Closer] 는 다음과 같이 정의됩니다.

| 위치 | 설명 |
|---|---|
| [!UICONTROL Starter] | 이 위치는 접점이 전환 경로의 첫 번째 터치인지 여부를 나타냅니다. |
| [!UICONTROL Player] | 이 위치는 접점이 전환으로 이어지는 첫 번째 터치인지 마지막 터치인지 여부를 나타냅니다. |
| [!UICONTROL Closer] | 이 위치는 접점이 전환 전 마지막 터치인지 여부를 나타냅니다. |


### [!UICONTROL Top conversion paths]

다음 [!UICONTROL Top conversion paths] 시각화는 선택한 속성 모델을 기반으로 상위 5개의 전환 경로를 보여 줍니다.

각 전환 경로에 대해 다음을 확인합니다.

* 영향을 미치는 채널의 수,
* 총 속성 경로,
* 이 전환 경로에 대한 속성 경로와 총 속성 경로의 백분율,
* 각 채널에 대해 속성 모델 기여도 백분율 및
* 이러한 채널 속성 모델 기여도의 합계입니다.


## [!UICONTROL Diagnostics]

진단 탭에 다음에 대한 위젯이 표시됩니다.

* [!UICONTROL Model Assessment] 시각화를 통해 실제 변환과 예측 또는 잔차 변환을 분류할 수 있습니다.

  시각화를 분류하려면 다음을 선택합니다. **[!UICONTROL Actual vs. Predicted]** 또는 **[!UICONTROL Residuals]** 다음에서 **[!UICONTROL Breakdown]** 목록을 표시합니다.

* [!UICONTROL Model fitting metrics] 각 전환 지표에 대해 다음 열을 보여 주는 표:

   * 실제 전환

   * 모델 전환

   * 잔차 변환(실제 변환과 모델 변환 간의 차이)

   * 모델 품질 점수 값:

      * 자료가 회귀 모형(적합도)에 얼마나 잘 부합하는지를 알려주는 R2(R-제곱)이다.

      * MAPE(Mean Absolute Percentage Error): 예측 정확도를 측정하기 위해 가장 일반적으로 사용되는 KPI 중 하나이며 예측 오류를 실제 값의 백분율로 표시합니다.

      * RMSE(제곱 평균 제곱근 오차): 오차의 제곱에 따라 가중치가 적용된 평균 오차를 보여 줍니다.

  테이블에 대한 데이터가 포함된 CSV 파일을 다운로드하려면 다음을 선택합니다. ![다운로드](../assets/icons/Download.svg).

* [!UICONTROL Touchpoint effectiveness] Attribution AI 알고리즘 모델의 결과를 나타내는 표입니다. 이 테이블의 데이터는 특정 기간 동안만 생성됩니다. 선택 **[!UICONTROL As of *xx/xx/xx, xx:xx TZ *]**![정보](../assets/icons/InfoOutline.svg) 을 참조하십시오.

  시각화는 다음 순서로 표시됩니다. [!UICONTROL Efficiency measure] ![내림차순](../assets/icons/SortOrderDown.svg), 각 터치포인트에 대해:

   * [!UICONTROL Paths touched]: 전환된 경로의 비율과 전환되지 않은 경로의 비율을 시각화합니다. 접점의 경우 속성 전환율이 높으면 더 많은 속성 전환을 볼 수 있습니다. 이 비율은 전환으로 이어지는 경로의 백분율과 전환으로 이어지는 경로의 백분율을 비교합니다 *아님* 전환으로 이어집니다.
   * [!UICONTROL Efficiency measure]: 알고리즘 속성 모델에 의해 생성된 효율성 측정은 접점 볼륨에 관계없이 전환에 대한 접점의 상대적 중요성을 나타냅니다. 효율은 1~5의 척도로 측정됩니다. 더 높은 접점 볼륨이 더 높은 효율성 측정을 보장하지는 않습니다.
   * [!UICONTROL Total volume]: 사용자가 터치포인트를 터치한 총 횟수입니다. 이 숫자는 전환을 수행하는 경로와 경로에 표시되는 터치포인트를 포함합니다 *아님* 결과적으로 전환됩니다.

![진단](../assets/model-insights-diagnostics.png)


## [!UICONTROL Historical overview]

내역 개요 탭에는 다음에 대한 위젯이 표시됩니다.

* 회계 분기 및 제품별 전환 및 소비.

* 채널별 소비.

* 접점 사용.

  이 위젯에 대해 표시할 대체 지출 기반 채널을 선택할 수 있습니다. 다음 위치에서 채널 선택 **[!UICONTROL Channels]**.

* 접점 볼륨.

  이 위젯에 대해 표시할 대체 볼륨 기반 채널을 선택할 수 있습니다. 다음 위치에서 채널 선택 **[!UICONTROL Channels]**.

![모델 - 기록 개요](../assets/model-insights-historical-overview.png)
