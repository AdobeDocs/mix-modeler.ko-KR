---
title: 모델 인사이트
description: Mix Modeler 시 기록 개요, 모델 통찰력 및 모델 품질과 같은 모델에 대한 세부 정보를 얻는 방법에 대해 알아봅니다.
feature: Models
exl-id: d99852f9-ba0d-4a2e-b5f3-ca0efe6002fd
source-git-commit: d4a500de13272f0b07827a0df4a386d3d757403b
workflow-type: tm+mt
source-wordcount: '1539'
ht-degree: 0%

---

# 모델 인사이트

모델 인사이트를 보려면 Mix Modeler의 ![모델](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** 인터페이스에서 다음을 수행합니다.

1. **[!UICONTROL Models]** 테이블에서 **[!UICONTROL Last run status]**&#x200B;이(가) <span style="color:green">●</span>인 모델의 이름을 선택하십시오. **[!UICONTROL Success]**.

1. 컨텍스트 메뉴에서 **[!UICONTROL Model Insights]**&#x200B;을(를) 선택합니다.

![모델 인사이트 탭 모음](/help/assets/model-insights-tabbar.png)

지정된 모델이 마지막으로 새로 고쳐지고 네 개의 탭을 사용하여 시각화가 표시되는지 확인합니다. [모델 인사이트](#model-insights), [속성](#attribution), [요소](#factors), [진단](#diagnostics) 및 [기록 개요](#historical-overview).

각 탭의 시각화의 기반이 되는 날짜 기간을 변경할 수 있습니다. 날짜 기간을 입력하거나 ![달력](/help/assets/icons/Calendar.svg)을 선택하여 날짜 기간을 선택하십시오.

## [!UICONTROL Model insights]

모델 인사이트 탭에는 [날짜 및 기본 미디어별 기여도](#contribution-by-date-and-base-media), [채널별 기여도](#contribution-by-channel), [마케팅 성과 요약](#marketing-performance-summary) 및 [한계 응답 곡선](#marginal-response-curves)에 대한 시각화가 표시됩니다. 탭은 [접점 분류](#touchppint-breakdown) 테이블도 제공합니다.

![모델 - 모델 인사이트](/help/assets/model-insights-insights.png)

* 각 시각화의 개별 차트 요소 위로 마우스를 가져가면 자세한 내용이 포함된 팝오버를 표시할 수 있습니다.

* 시각화에 대한 데이터가 포함된 CSV 파일을 다운로드하려면 ![다운로드](/help/assets/icons/Download.svg)를 선택하십시오.

* Microsoft® Excel 형식으로 전체 모델 인사이트 데이터를 다운로드하려면 ![다운로드](/help/assets/icons/Download.svg) **[!UICONTROL Download data]**&#x200B;를 선택하십시오.


### 날짜 및 기본 미디어별 기여도.

누적 그래프는 맨 아래에 기준, 중간에 비지출 채널 및 맨 위에 지출 채널의 순서로 정렬됩니다.

### 채널별 기여도

도넛 시각화는 채널별 기여도 분포를 보여 줍니다.

### 마케팅 성과 요약.

채널별 ROI 성능을 표시하는 가로 막대 그래프입니다.

### 한계 응답 곡선.

라인 차트는 마케팅 채널에 대한 투자로 생성된 한계 수익을 시각화하고 비교합니다.  증분 수익이 증분 지출보다 작은 손익분기점을 식별합니다. 따라서 이 시각화는 마케팅 투자의 영향이 감소하기 시작하는 시기를 이해하는 데 도움이 됩니다.

커브, 손익분기점 및 해당 값은 선택한 데이터 범위와 선택한 채널을 기반으로 계산됩니다.

채널을 변경하려면:

* **[!UICONTROL Channel]** 드롭다운 메뉴에서 채널을 선택하여 특정 채널에 대한 시각화를 업데이트합니다.


### 접점 분류

접점 분류 테이블에는 주별 기준으로 모든 또는 선택한 채널에 대한 접점 분류가 표시됩니다.

![접점 분류](../assets/touchpoint-breakdown.png)

다음 열을 사용할 수 있습니다.

| 열 | 설명 |
|---|---|
| **[!UICONTROL Date range]** | 보고할 주입니다. |
| **[!UICONTROL Touchpoint]** | 특정 터치포인트 채널. |
| **[!UICONTROL ROI]** | (**[!UICONTROL Revenue]** - **[!UICONTROL Spend]**) / **[!UICONTROL Spend]**&#x200B;의 백분율입니다. |
| **[!UICONTROL Revenue]** | 날짜 범위에 대한 매출입니다. |
| **[!UICONTROL CPA]** | **[!UICONTROL Spend]** / **[!UICONTROL Conversions]**. |
| **[!UICONTROL Conversions]** | 날짜 범위에 대한 전환입니다. |
| **[!UICONTROL Spend]** | 데이터 범위에 대한 지출입니다. |

특정 채널 또는 모든 채널을 선택하려면 **[!UICONTROL View]** 드롭다운 메뉴에서 선택하십시오.

접점 분류 테이블의 내용을 다운로드하려면 ![다운로드](/help/assets/icons/Download.svg) **[!UICONTROL Download CSV]**&#x200B;을(를) 선택하십시오.


## [!UICONTROL Attribution]

>[!NOTE]
>
>속성 탭은 MTA 활성화 모델에만 사용할 수 있습니다.


[!UICONTROL Attribution] 탭을 사용하여 이벤트 수준 데이터가 있는 터치포인트 및 마케팅 캠페인의 효과를 이해할 수 있습니다.  [모델 만들기](create.md)를 참조하세요.

지원되는 속성 모델은 다음과 같습니다.

* Mix Modeler에서 선택한 모델 기반:
   * 알고리즘 - 영향
   * 알고리즘 - 증분
* 규칙 기반:
   * 가치 감소 단위
   * 첫 번째 터치
   * 마지막 터치
   * 선형
   * U자형

Mix Modeler의 다중 터치 속성 기능에 대한 소개는 [다중 터치 속성](../get-started/about.md#multi-touch-attribution)을 참조하십시오.

**[!UICONTROL Attribution Model]** 드롭다운 메뉴에서 속성 모델을 하나 이상 선택합니다. 선택한 속성 모델은 속성 탭의 모든 시각화에 적용됩니다.

![속성](/help/assets/model-insights-attribution.png)

Mix Modeler 멀티 터치 속성 세분화된 이벤트 점수는 전체 Mix Modeler 점수 및 ROI에 맞게 조정됩니다. 이러한 점수는 Experience Platform에서 데이터 세트로 사용할 수도 있습니다.

속성 탭은 다음 시각화로 구성됩니다.

### [!UICONTROL Overview]

[!UICONTROL Overview] 시각화는 선택한 속성 모델에 대한 전환 합계 및 백분율을 보여 줍니다. 모델을 더 선택하면 시각화에 범례에 해당하는 자체 색상이 있는 원이 더 추가됩니다.

속성 모델에 대한 세부 사항이 있는 팝업을 보려면 시각화의 원 위로 마우스를 가져갑니다.

### [!UICONTROL Trends]

[!UICONTROL Daily trends], [!UICONTROL Weekly trends] 또는 [!UICONTROL Monthly trends] 시각화는 선택한 속성 모델에 대해 일별, 주별 또는 월별 전환 트렌드를 표시합니다.

기간을 선택하려면 ![자세히](/help/assets/icons/More.svg)에서 **[!UICONTROL Daily trends]**, **[!UICONTROL Weekly trends]** 또는 **[!UICONTROL Monthly trends]**&#x200B;을(를) 선택하십시오.

세부 정보를 보려면 특정 속성 모델의 데이터 라인 위로 마우스를 가져가 해당 데이터에 대한 총 전환 수를 표시하는 팝오버를 표시합니다.

### [!UICONTROL Breakdown]

[!UICONTROL Breakdown] 시각화는 선택한 각 속성 모델에 대한 전환의 채널 또는 터치포인트별 분류입니다. 이 시각화는 각 채널 또는 터치포인트의 효과에 대한 결정을 내리는 데 도움이 될 수 있습니다.

분류 유형을 선택하려면 ![자세히](/help/assets/icons/More.svg)에서 **[!UICONTROL Breakdown by channel]** 또는 **[!UICONTROL Breakdown by touchpoint]**&#x200B;을(를) 선택하십시오.

세부 정보를 보려면 차트 요소 위로 마우스를 가져갑니다.

### [!UICONTROL Top campaigns]

상위 캠페인 시각화는 캠페인 이름, 채널, 미디어 유형 및 증분 전환에 대한 열이 있는 상위 캠페인의 테이블을 표시합니다. 이 시각화는 주어진 채널에 대한 특정 캠페인의 효과를 팀에 알리고 추가로 투자해야 하는 캠페인에 대한 통찰력을 제공하는 데 도움이 될 수 있습니다.

채널, 미디어 유형 또↑ 증분 전환에 ↓ 오름차순 또는 내림차순으로 테이블을 정렬하려면 열 헤더를 선택하고 정렬을 토글합니다.

별도의 대화 상자에서 테이블을 확장하려면 ![자세히](/help/assets/icons/More.svg)에서 **[!UICONTROL Expand]**&#x200B;을(를) 선택합니다.

확장된 [상위 캠페인] 대화 상자에는 다음과 같은 추가 열이 있는 동일한 테이블이 표시됩니다.

* 증분 전환
* 영향을 받은 전환
* 첫 번째 터치 전환
* 마지막 터치 전환

  추가 열 헤더를 각각 선택하여 테이블을 오름차순 또는 내림차순으로 정렬할 수 있습니다.

확장된 [최상위 캠페인] 대화 상자를 닫으려면 **[!UICONTROL Close]**&#x200B;을(를) 선택합니다.


### [!UICONTROL Breakdown by touchpoint position]

[!UICONTROL Breakdown by touchpoint position] 시각화는 모든 전환 경로에서 접점 및 접점 위치별 속성 전환의 분류입니다. 이 차트는 터치포인트가 나머지 위치와 다른 위치보다 한 위치에서 더 잘 기여하는지 비교하는 데 도움이 됩니다.

>[!NOTE]
>
>모든 접점 및 위치에서 속성 모델에 대한 백분율 기여도의 합계는 100이어야 합니다.


위치 [!UICONTROL Starter], [!UICONTROL Player] 및 [!UICONTROL Closer]은(는) 다음과 같이 정의됩니다.

| 위치 | 설명 |
|---|---|
| [!UICONTROL Starter] | 이 위치는 접점이 전환 경로의 첫 번째 터치인지 여부를 나타냅니다. |
| [!UICONTROL Player] | 이 위치는 접점이 전환으로 이어지는 첫 번째 터치인지 마지막 터치인지 여부를 나타냅니다. |
| [!UICONTROL Closer] | 이 위치는 접점이 전환 전 마지막 터치인지 여부를 나타냅니다. |


### [!UICONTROL Top conversion paths]

[!UICONTROL Top conversion paths] 시각화는 선택한 속성 모델을 기반으로 상위 5개의 전환 경로를 표시합니다.

각 전환 경로에 대해 다음을 확인합니다.

* 영향을 미치는 채널의 수,
* 총 속성 경로,
* 이 전환 경로에 대한 속성 경로와 총 속성 경로의 백분율,
* 각 채널에 대해 속성 모델 기여도 백분율 및
* 이러한 채널 속성 모델 기여도의 합계입니다.

## **[!UICONTROL Factors]**

요소 탭에는 외부 요소 관련 통찰력이 표시됩니다.

![요소](/help/assets/factors.png)

이 시각화는 다양한 내부 및 외부 요인이 전환 기준선에 미치는 증분 효과를 이해하는 데 도움이 됩니다. 예를 들어, 경제 상황 또는 홍보 활동.


테이블에 대한 데이터가 포함된 CSV 파일을 다운로드하려면 ![다운로드](/help/assets/icons/Download.svg)를 선택합니다.

데이터를 사용할 수 없으면 ![TableAndChart](/help/assets/icons/TableAndChart.svg) **[!UICONTROL No data is available, you may need to retrain your model, or change the date range to view insights]** 메시지가 표시됩니다.

## [!UICONTROL Diagnostics]

진단 탭에 다음에 대한 시각화가 표시됩니다.

* [!UICONTROL Model Assessment] 시각화(실제 변환과 예측 또는 잔차 변환을 분류할 수 있음)

  시각화를 분류하려면 **[!UICONTROL Breakdown]** 목록에서 **[!UICONTROL Actual vs. Predicted]** 또는 **[!UICONTROL Residuals]**&#x200B;을(를) 선택하십시오.

* 각 전환 지표에 대해 다음 열을 표시하는 [!UICONTROL Model fitting metrics] 테이블:

   * 실제 전환

   * 모델 전환

   * 잔차 변환(실제 변환과 모델 변환 간의 차이)

   * 모델 품질 점수 값:

      * 자료가 회귀 모형(적합도)에 얼마나 잘 부합하는지를 알려주는 R2(R-제곱)이다.

      * MAPE(Mean Absolute Percentage Error): 예측 정확도를 측정하기 위해 가장 일반적으로 사용되는 KPI 중 하나이며 예측 오류를 실제 값의 백분율로 표시합니다.

      * RMSE(제곱 평균 제곱근 오차): 오차의 제곱에 따라 가중치가 적용된 평균 오차를 보여 줍니다.

  테이블에 대한 데이터가 포함된 CSV 파일을 다운로드하려면 ![다운로드](/help/assets/icons/Download.svg)를 선택합니다.

* Attribution AI 알고리즘 모델의 결과를 나타내는 [!UICONTROL Touchpoint effectiveness] 테이블입니다. 이 테이블의 데이터는 특정 기간 동안만 생성됩니다. 자세한 내용은 **[!UICONTROL As of *xx/xx/xx, xx:xx TZ *]**![정보](/help/assets/icons/InfoOutline.svg)를 선택하십시오.

  시각화는 각 터치포인트에 대해 내림차순 [!UICONTROL Efficiency measure] ![내림차순](/help/assets/icons/SortOrderDown.svg)으로 표시됩니다.

   * [!UICONTROL Paths touched]: 전환된 경로의 비율과 전환되지 않은 경로의 비율을 시각화합니다. 접점의 경우 속성 전환율이 높으면 더 많은 속성 전환을 볼 수 있습니다. 이 비율은 전환으로 이어지는 경로의 비율과 전환으로 이어지는 *아닌*&#x200B;경로의 비율을 비교합니다.
   * [!UICONTROL Efficiency measure]: 알고리즘 속성 모델에 의해 생성된 효율성 측정은 접점 볼륨에 관계없이 전환에 대한 접점의 상대적 중요성을 나타냅니다. 효율은 1~5의 척도로 측정됩니다. 더 높은 접점 볼륨이 더 높은 효율성 측정을 보장하지는 않습니다.
   * [!UICONTROL Total volume]: 사용자가 터치포인트를 터치한 총 횟수입니다. 이 숫자는 전환을 수행하는 경로와 전환을 수행하는 경로 *not*&#x200B;에 표시되는 터치포인트를 포함합니다.

![진단](/help/assets/model-insights-diagnostics.png)


## [!UICONTROL Historical overview]

내역 개요 탭에는 다음에 대한 시각화가 표시됩니다.

* 회계 분기 및 제품별 전환 및 소비.

* 채널별 소비.

* 접점 사용.

  이 시각화에 표시할 대체 지출 기반 채널을 선택할 수 있습니다. **[!UICONTROL Channels]**&#x200B;에서 채널을 선택하십시오.

* 접점 볼륨.

  이 시각화에 표시할 대체 볼륨 기반 채널을 선택할 수 있습니다. **[!UICONTROL Channels]**&#x200B;에서 채널을 선택하십시오.

![모델 - 이전 개요](/help/assets/model-insights-historical-overview.png)

## **[!UICONTROL Edit]**

모델의 이름, 설명 및 교육 및 채점 일정을 편집할 수 있습니다.

1. ![편집](/help/assets/icons/Edit.svg) 편집 선택

1. **[!UICONTROL Edit model]** 대화 상자에서:

   * 새 **[!UICONTROL Name]** 및 **[!UICONTROL Description]**&#x200B;을(를) 입력하십시오.

   * 예약을 사용하려면 **[!UICONTROL Status]**&#x200B;을(를) 사용하도록 설정하십시오. 교육되고 점수가 매겨진 모델만 예약할 수 있습니다.

      1. **[!UICONTROL Scoring frequency]** 선택:

         * **[!UICONTROL Daily]**: 올바른 시간(예: `05:22 pm`)을 입력하거나 ![시계](/help/assets/icons/Clock.svg)를 사용하십시오.
         * **[!UICONTROL Weekly]**: 요일을 선택하고 올바른 시간(예: `05:22 pm`)을 입력하거나 ![시계](/help/assets/icons/Clock.svg)를 사용하십시오.
         * **[!UICONTROL Monthly]**: 모든 드롭다운 메뉴에서 요일을 선택하고 올바른 시간(예: `05:22 pm`)을 입력하거나 ![시계](/help/assets/icons/Clock.svg)를 사용하십시오.

      1. 드롭다운 메뉴에서 **[!UICONTROL Training frequency]**&#x200B;을(를) 선택합니다. **[!UICONTROL Monthly]**, **[!UICONTROL Quarterly]**, **[!UICONTROL Yearly]** 또는 **[!UICONTROL None]**.

     ![모델 편집](../assets/model-edit.png)

1. **[!UICONTROL Save]**&#x200B;를 선택합니다.
