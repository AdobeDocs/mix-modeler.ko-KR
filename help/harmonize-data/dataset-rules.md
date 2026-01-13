---
title: 데이터 세트 규칙
description: Mix Modeler에서 데이터를 조화롭게 만드는 과정에서 사용할 데이터 세트 규칙을 정의하는 방법을 알아봅니다.
feature: Harmonized Data, Dataset Rules
exl-id: 57d7940a-2900-4814-a30d-bb02bff7615d
source-git-commit: b631cf8d06fe71d9f5ca547923eb3237c677a915
workflow-type: tm+mt
source-wordcount: '1696'
ht-degree: 0%

---

# 데이터 세트 규칙

데이터 세트 규칙은 조화 된 필드를 Mix Modeler에서 수집한 데이터의 필드와 매핑하는 데 도움이 됩니다.

* Adobe Experience Platform에서 수집한 집계 데이터의 경우 사용 가능한 데이터 세트 필드 중 하나 이상을 적절한 조화된 필드에 매핑합니다.
* 이벤트 데이터의 경우, 직접 또는 조건을 사용하여 하나 이상의 조정된 필드를 데이터 세트의 필드에 개별적으로 매핑할 수 있습니다.


## 데이터 세트 규칙 관리

Mix Modeler 인터페이스에서 사용 가능한 데이터 세트 규칙 표를 보려면 다음을 수행하십시오.

1. 왼쪽 레일에서 ![DataSearch](/help/assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]**&#x200B;을(를) 선택합니다.

1. 상단 표시줄에서 **[!UICONTROL Dataset rules]**&#x200B;을(를) 선택합니다. 데이터 세트 규칙 표가 표시됩니다.

![검색](/help/assets/icons/Search.svg) **[!UICONTROL _데이터 세트 이름 입력_]**&#x200B;을 사용하여 데이터 세트를 빠르게 검색할 수 있습니다.

테이블 열은 데이터 세트 규칙에 대한 세부 사항을 지정합니다.

| 열 이름 | 세부 사항 |
| ---------------------- | ----------|
| 데이터 세트 | 데이터 세트의 이름입니다.  데이터 집합에 대한 작업을 선택하려면 ![자세히](/help/assets/icons/More.svg)를 사용하세요. 다음과 같은 작업을 수행할 수 있습니다.<ul><li>데이터 집합 규칙 구성을 보려면 ![미리 보기](/help/assets/icons/Preview.svg) **[!UICONTROL View]**&#x200B;하세요. 모든 필드가 비활성화됩니다.</li><li>데이터 집합 규칙 구성을 편집하려면 ![편집](/help/assets/icons/Edit.svg) **[!UICONTROL Edit]**&#x200B;하세요.</li><li>데이터 집합 규칙 구성을 삭제하려면 ![삭제](/help/assets/icons/Delete.svg) **[!UICONTROL Delete]**&#x200B;하십시오. 데이터 세트 삭제 대화 상자에서 삭제를 확인하라는 메시지가 표시됩니다. 데이터 집합 규칙 구성을 영구적으로 삭제하려면 **[!UICONTROL Delete]**&#x200B;을(를) 선택하십시오.</li><ul> |
| 소스 | 데이터 세트의 소스: Adobe Analytics, 경험 이벤트, 요약(집계) 또는 소비자 경험 이벤트. |
| 스키마 | 데이터 세트가 준수하는 스키마. 스키마 이름을 빠르게 선택하여 ![스키마](/help/assets/icons/Schemas.svg) [스키마](../ingest-data/schemas.md)의 스키마 편집기의 새 탭에서 스키마를 열 수 있습니다. |
| 세부기간 | 데이터 집합에 있는 데이터의 세부기간입니다. 가능한 값은 일별, 주별, 월별 또는 연도별입니다. |
| 주의 시작 | 특정 데이터 세트에 대해 새 주의 시작으로 간주되는 요일을 지정합니다. |
| 상태 | 필드의 상태: <p><span style="color:gray">●</span> 초안 또는 <p><span style="color:green">●</span> 활성 |
| 마지막 수정일 | 데이터 집합 규칙을 마지막으로 수정한 데이터 및 시간입니다. |

{style="table-layout:auto"}

### 데이터 세트 규칙 만들기

데이터 집합 규칙을 만들려면 Mix Modeler의 ![DataSearch](/help/assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Dataset rules]** 인터페이스에서 **[!UICONTROL Create a dataset rule]** 마법사의 **[!UICONTROL Dataset rules configuration]**&#x200B;을(를) 선택하십시오.

**[!UICONTROL Create]** 화면에서

1. **[!UICONTROL Dataset details]**&#x200B;에서 구성을 시작하려면 **[!UICONTROL Select dataset]**&#x200B;에서 데이터 집합을 선택하십시오. 목록에서 데이터 세트는 **[!UICONTROL Consumer Experience Events]**, **[!UICONTROL Adobe Analytics]**, **[!UICONTROL Experience Event]** 및 **[!UICONTROL Summary]**(으)로 분류됩니다.

1. **[!UICONTROL Start of the week]**&#x200B;에 대한 요일을 선택하십시오.

1. **[!UICONTROL Daily]**&#x200B;에 대해 **[!UICONTROL Weekly]**, **[!UICONTROL Monthly]**, **[!UICONTROL Yearly]** 또는 **[!UICONTROL Granularity]**&#x200B;을(를) 선택하십시오.

1. **[!UICONTROL Summary]** 범주의 데이터 집합을 선택한 경우 **[!UICONTROL Aggregation]**&#x200B;에 대해 **[!UICONTROL Replacement]** 또는 **[!UICONTROL Data restatement is by]**&#x200B;을(를) 선택하십시오.

   게시자와 함께 작업하면 상당한 지출이 수반되는 경우가 많기 때문에 게시자의 보고 데이터는 마케팅 분석가에게 매우 중요하며 보고 데이터를 변경하면 통찰력과 투자 계획이 매우 달라질 수 있습니다. 또한 마케팅 분석가는 올바른 통찰력을 도출하고 설득력 있는 제안을 제시하여 관련자의 신뢰를 얻을 수 있는 정확한 데이터가 필요합니다. 그러나 Google 및 Facebook과 같은 이러한 게시자는 데이터를 조정할 때 보고 데이터를 다시 표시하거나 삭제하는 경우가 많습니다. 대부분의 변경 사항에 대한 시간대는 보고된 미디어 성능에서 7일 이내입니다. 데이터에 대한 추가 변경은 30일 이내에 가능합니다. 일반적으로 30일이 지나면 책이 폐쇄되고 자료가 완성되는 것으로 간주된다.

   Mix Modeler은 데이터 재정의를 지원합니다. 보고, 모델링 및 계획에 사용되는 데이터가 정확한지 확인하기 위해 또한 이 데이터는 브랜드 및 마케팅 분석가의 기대와 요구를 지원할 수 있습니다.

   요약 데이터의 다시 기술된 행을 Experience Platform 데이터 세트에서 증분 행으로 보낼 수 있으며 조화 서비스는 다시 기술된 데이터로 조화 데이터 세트를 업데이트합니다. 마찬가지로, 조화 서비스에 반영해야 하는 요약 데이터의 행을 제거할 수도 있습니다.

1. **[!UICONTROL Map to harmonized fields]** 섹션에서:

   1. **[!UICONTROL Standard harmonized field]**&#x200B;에서 통합 필드를 선택하십시오.

   1. 선택한 조화로운 필드가 유형 지표인 경우:

      1. **[!UICONTROL Count]**&#x200B;에서 **[!UICONTROL Sum]** 또는 **[!UICONTROL Mapping type]**&#x200B;을(를) 선택합니다.

      1. 기본적으로 통합 필드를 매핑할 **[!UICONTROL *AEP 데이터 세트 필드&#x200B;*]**를 선택하십시오.

   1. 선택한 필드가 차원 유형인 경우:

      1. **[!UICONTROL Map Into]**&#x200B;에서 **[!UICONTROL Case]** 또는 **[!UICONTROL Mapping type]**&#x200B;을(를) 선택합니다.

      1. **[!UICONTROL Map Into]**&#x200B;을(를) 선택한 경우 **[!UICONTROL Field]**&#x200B;과(와) **[!UICONTROL *AEP 데이터 세트 필드&#x200B;*]**또는&#x200B;**[!UICONTROL Value]**을(를) 선택하고 기본적으로 조화 필드를 데이터 세트 필드 또는 입력된 값에 매핑합니다.

      1. **[!UICONTROL Case]**&#x200B;을(를) 선택한 경우 **[!UICONTROL Field]** 및 **[!UICONTROL *AEP 데이터 세트 필드&#x200B;*]**또는&#x200B;**[!UICONTROL Value]**을(를) 선택하고 기본적으로 조화 필드를 데이터 세트 필드 또는 입력된 값에 매핑합니다.

         1. 값을 명시적으로 설정하려면 하나 이상의 조건으로 구성된 하나 이상의 사례를 정의합니다. 각 조건은 특정 **[!UICONTROL *AEP 데이터 세트 필드&#x200B;*]**에 대해&#x200B;**[!UICONTROL Exists]**또는&#x200B;**[!UICONTROL Not Exists]**인지 또는&#x200B;**[!UICONTROL Contains]**입력 값 입력&#x200B;**[!UICONTROL Not Contains]**에 입력한 값이&#x200B;**[!UICONTROL Equals]**,**[!UICONTROL Not Equals]**,**[!UICONTROL Starts With]**,**[!UICONTROL Ends With]**,**[!UICONTROL * 또는 *]**&#x200B;인지 여부를 확인할 수 있습니다.

         1. 다른 서비스 케이스를 추가하려면 ![추가](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add case]**&#x200B;를 선택하고 다른 조건을 추가하려면 ![추가](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add condition]**&#x200B;를 선택합니다.

         1. 서비스 케이스 또는 조건을 삭제하려면 해당 컨테이너에서 ![닫기](/help/assets/icons/Close.svg)를 선택합니다.

         1. 서비스 케이스에 조건을 적용할지 또는 모두 적용할지 여부를 선택하려면 **[!UICONTROL Any of]** 또는 **[!UICONTROL All of]**&#x200B;을(를) 선택하십시오.

         1. 사례에 대한 결과 값을 설정하려면 **[!UICONTROL Then]**&#x200B;에 값을 입력하십시오.

      아래 예

      * **[!UICONTROL Map Into]** **[!UICONTROL Mapping type]**&#x200B;을(를) 사용하여 **[!UICONTROL Channel Type At Source]** harmonized 필드를 **[!UICONTROL channel_type]** 데이터 세트의 **[!DNL Luma Transactions]** 필드에 매핑합니다.

      * **[!UICONTROL Case]** **[!UICONTROL Mapping type]**&#x200B;을(를) 사용하여 **[!UICONTROL marketing.campaignName]** 데이터 집합에 있는 **[!DNL Luma Transactions]** 필드의 값을 **[!UICONTROL Campaign]** 조화 필드에 조건부로 매핑합니다. Campaign harmonized 필드가 다음으로 설정됨:

         * `Black Friday`이(가) **[!UICONTROL marketing.campaignName]** 또는 `_black_friday`인 경우 `BlackFriday`.
         * 다른 모든 경우에는 **[!UICONTROL marketing.campaignName]**&#x200B;의 값으로 설정됩니다.

        ![데이터 집합 규칙 이벤트](/help/assets/dataset-create-event.png)

      요약 데이터 세트에서 표준 조화 필드를 매핑하면 Mix Modeler은 해당 Experience Platform 데이터 세트 필드를 추론합니다. 성공 시:

      * 필드가 유형 차원이면 **[!UICONTROL Map into]**&#x200B;이(가) **[!UICONTROL Mapping type]**(으)로 선택됩니다.
      * 필드가 유형 지표인 경우 **[!UICONTROL Sum]**&#x200B;이(가) **[!UICONTROL Mapping type]**(으)로 선택됩니다.
      * **[!UICONTROL Field]**&#x200B;이(가) **[!UICONTROL Default]** 매핑 유형으로 선택되었습니다.
      * 해당 Experience Platform 데이터 세트 필드는 *AEP 데이터 세트 필드*&#x200B;에 대해 자동으로 삽입됩니다.

      제안된 값이 올바르지 않거나 특정 사용 사례를 지원하지 않는 경우 해당 값을 변경할 수 있습니다.

1. 추가 필드를 정의하려면 ![추가](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add field]**&#x200B;을(를) 선택하십시오.

완료되면 규칙의 초안 버전을 저장하려면 **[!UICONTROL Save as draft]**&#x200B;을(를) 선택하고 규칙을 저장하고 활성화하려면 **[!UICONTROL Save]**&#x200B;을(를) 선택합니다. 규칙 구성을 취소하려면 **[!UICONTROL Cancel]**&#x200B;을(를) 선택하십시오.

>[!NOTE]
>
>요약 데이터 세트 규칙에 대한 전용 **[!UICONTROL Map to harmonized fields]** 경험은 더 이상 사용되지 않습니다. 이제 모든 데이터 세트 규칙이 데이터 세트 유형에 관계없이 유사한 **[!UICONTROL Map to harmonized fields]** 경험을 사용합니다. 더 이상 사용되지 않는 **[!UICONTROL Map to harmonized fields]** 경험을 사용하여 규칙을 정의한 요약 데이터 세트의 경우 일반 **[!UICONTROL Map to harmonized field]** 경험에 대해 이러한 규칙을 확인할 수 있습니다.
>



### 데이터 세트 규칙 편집

데이터 집합 규칙을 편집하려면 Mix Modeler의 ![DataSearch](/help/assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Dataset rules]** 인터페이스에서 다음을 수행하십시오.

1. 편집할 데이터 세트 규칙에 대해 ![ 열에서 ](/help/assets/icons/More.svg)자세히&#x200B;**[!UICONTROL Dataset]**&#x200B;를 선택합니다.
1. 컨텍스트 메뉴에서 ![편집](/help/assets/icons/Edit.svg) **[!UICONTROL Edit]**&#x200B;을(를) 선택하여 데이터 집합 규칙 편집을 시작합니다. 자세한 내용은 [데이터 집합 규칙 만들기](#create-a-dataset-rule)를 참조하세요.


### 데이터 세트 규칙 삭제

데이터 집합 규칙을 삭제하려면 Mix Modeler의 ![DataSearch](/help/assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Dataset rules]** 인터페이스에서 다음을 수행하십시오.

1. 삭제할 데이터 세트 규칙에 대해 ![ 열에서 ](/help/assets/icons/More.svg)자세히&#x200B;**[!UICONTROL Dataset]**&#x200B;를 선택하십시오.
1. 컨텍스트 메뉴에서 ![삭제](/help/assets/icons/Delete.svg) **[!UICONTROL Delete]**&#x200B;을(를) 선택하여 데이터 집합 규칙을 삭제합니다. 확인을 묻는 메시지가 표시됩니다. 선택한 데이터 집합 규칙을 영구적으로 삭제하려면 **[!UICONTROL Delete]**&#x200B;을(를) 선택하십시오.



## 데이터 동기화

데이터 세트 규칙의 논리를 적용하면서 조화된 데이터와 요약 및/또는 이벤트 데이터 세트 간에 데이터를 동기화하려면 다음을 수행하십시오.

1. **[!UICONTROL Sync data]**&#x200B;를 선택합니다.

1. **[!UICONTROL Sync data for dataset rules]** 대화 상자에서 다음 중 하나를 선택합니다
   * **[!UICONTROL Refresh harmonized data for summary datasets]**,
   * **[!UICONTROL Refresh harmonized data for event datasets]** 또는
   * **[!UICONTROL Refresh harmonized data for both summary + event datasets]**.

1. 통합 데이터와 데이터 집합의 데이터 간에 정의된 데이터 집합 규칙을 기반으로 동기화를 시작하려면 **[!UICONTROL Sync]**&#x200B;을(를) 선택하십시오. 동기화를 취소하려면 **[!UICONTROL Cancel]**&#x200B;을(를) 선택하십시오.

   ![데이터 동기화](/help/assets/sync-data.png)


## 데이터 병합 환경 설정

>[!NOTE]
>
>[!BADGE 베타]{type=Informative} 데이터 병합 환경 설정은 Beta 기능이며 기능은 변경될 수 있습니다.

정확한 모델 예측을 위해 데이터 병합 환경 설정을 정의할 수 있습니다. 이 기능을 사용하면 요약 수준 및 이벤트 수준 데이터를 병합한 후 발생하는 충돌을 해결할 수 있습니다.

업데이트가 충돌하는 경우 기본 지표 환경 설정을 적용하도록 구성할 수 있습니다. 이 기본 지표는 다음 세 가지 옵션 중 하나일 수 있습니다.

* **[!UICONTROL Summary data]**
* **[!UICONTROL Sum of summary and event data]**
* **[!UICONTROL Event data]**

조화 중에 여러 데이터 소스가 지정된 채널에 대한 지표 필드를 업데이트하려고 하면 사용자가 구성한 기본 환경 설정이 적용됩니다. 이 환경 설정은 추가로 구성된 특정 지표 기반 환경 설정에 대해 재정의되지 않는 한 샌드박스 수준에서 적용됩니다.

**[!UICONTROL Metric based preferences]**&#x200B;에서 사용자는 특정 지표에 대한 특정 원본(**[!UICONTROL Summary]** 또는 **[!UICONTROL Event]**)과 해당 지표에 대한 해당 전환 유형을 구성할 수 있습니다.

일반적인 사용 사례는 다음과 같습니다.

* 동일한 광고 지표가 여러 데이터 세트에서 측정되고 보고되거나
* 일부 데이터 세트에서는 지표 측정이 불완전할 수 있지만 다른 데이터 세트는 특정 지표의 상위 집합일 수 있으므로 두 번 계산됩니다.

### 구성

데이터 병합 환경 설정을 구성하려면 다음 작업을 수행하십시오.


1. ![데이터 병합 환경 설정](/help/assets/icons/Merge.svg) [!BADGE 베타]을(를) 선택하십시오.

1. **[!UICONTROL Data merge preferences]** [!BADGE 베타]{type=Informative} 대화 상자:

   ![데이터 병합 환경 설정](/help/assets/data-merge-preferences.png)

   * **[!UICONTROL Default metric preference]** 선택. 선택한 기본 지표 환경 설정은 조화 중에 여러 데이터 소스가 지정된 채널에 대한 지표 필드를 업데이트할 때 적용됩니다. 특정 지표 기반 환경 설정에 대해 재정의되지 않는 한 환경 설정은 샌드박스 수준에서 적용됩니다. **[!UICONTROL Summary data]**, **[!UICONTROL Event data]** 및 **[!UICONTROL Sum of summary and event data]** 중에서 선택할 수 있습니다.

   * 특정 지표 기반 환경 설정을 추가하려면 다음 작업을 수행하십시오.

      1. ![더하기](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add a metric]**&#x200B;을(를) 선택합니다.
         1. **[!UICONTROL *지표 선택&#x200B;*]**목록에서 지표를 선택합니다.
         1. **[!UICONTROL CHANNELS]** 또는 **[!UICONTROL CONVERSION TYPES]**&#x200B;을(를) 선택하십시오. 목록에서 **[!UICONTROL All]** 또는 특정 채널 또는 전환 유형을 선택합니다.
         1. 데이터를 병합할 때 지표(및 모든 또는 선택한 채널)에 대해 요약 데이터나 이벤트 데이터를 선호하는지 여부를 지정하려면 **[!UICONTROL Summary]** 또는 **[!UICONTROL Event]**&#x200B;을(를) 선택하십시오.

         하나 이상의 채널 또는 전환 유형을 추가하려면 다음을 수행합니다.

         1. ![Plus](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add a channel]** 또는 ![Plus](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add a conversion type]**&#x200B;을(를) 선택하십시오.
         1. **[!UICONTROL Summary]** 또는&#x200B;**[!UICONTROL Event]**&#x200B;를 선택합니다.

         채널 또는 전환 유형을 삭제하려면 ![교차](/help/assets/icons/Close.svg)를 선택하세요.

      1. 더 구체적인 지표 기반 환경 설정을 추가하려면 이전 단계를 반복합니다.

   * 기존의 특정 지표 기반 환경 설정을 삭제하려면 ![삭제](/help/assets/icons/Delete.svg)를 선택하십시오.

1. **[!UICONTROL Save]**&#x200B;을(를) 선택하여 데이터 병합 환경 설정을 저장합니다. 데이터 재동기화가 시작됩니다. <br/>취소하려면 **[!UICONTROL Cancel]**&#x200B;을(를) 선택하십시오.

## 소스 데이터 세트 삭제

통합 데이터에서 사용되는 소스 데이터 집합을 삭제하면 해당 소스 데이터 집합의 기본 항목이 [[!UICONTROL Harmonized data]](/help/harmonize-data/overview.md)에서 제거됩니다. 그러나 삭제된 원본 데이터 집합이 있는 데이터 집합 규칙은 원본 데이터 집합이 삭제되었음을 나타내는 ![DataRemove](/help/assets/icons/DataRemove.svg) 아이콘과 함께 데이터 집합 규칙 구성 목록에 남아 있습니다. 자세한 내용을 보려면 다음 작업을 수행하십시오.

* 컨텍스트 메뉴에서 ![자세히](/help/assets/icons/More.svg) 및 ![미리 보기](/help/assets/icons/Preview.svg) **[!UICONTROL View]**을(를) 선택합니다.
**[!UICONTROL Dataset rule mapping - Fields]** 대화 상자에는 삭제된 원본 데이터 집합과 데이터 집합 규칙 구성에 사용된 필드에 대한 정보가 표시됩니다.

**[!UICONTROL Dataset rules]** 구성으로 돌아가면 하나 이상의 소스 데이터 세트가 삭제되었음을 설명하는 대화 상자가 표시됩니다. 조화된 데이터는 다음 애드혹 또는 예약된 동기화의 영향을 받습니다. 데이터 세트 규칙 구성을 검토하십시오.

다음 임시 동기화 또는 예약된 동기화 시 삭제된 소스 데이터 없이 조정된 데이터가 업데이트됩니다. 하지만 삭제된 소스 데이터 세트를 기준으로 데이터 세트 규칙을 삭제하라는 경고 대화 상자가 계속 표시됩니다. 이 경고를 통해 사용자는 삭제된 데이터 세트에서 영향을 받는 필드를 보고 평가할 수 있습니다. 또한 모든 모델에서 사용할 수 있는 마케팅 접점 또는 전환에 대한 영향을 결정합니다. 이 영향을 검토하고 완화했으면 데이터 세트 규칙 구성 목록에서 데이터 세트 규칙을 삭제해야 합니다.
