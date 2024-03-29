---
title: 데이터 세트 규칙
description: Mix Modeler에서 데이터를 조화롭게 만드는 과정에서 사용할 데이터 세트 규칙을 정의하는 방법을 알아봅니다.
feature: Harmonized Data, Dataset Rules
exl-id: 57d7940a-2900-4814-a30d-bb02bff7615d
source-git-commit: 86732fe30637aa72ced232d9f331a3cc64baa39b
workflow-type: tm+mt
source-wordcount: '980'
ht-degree: 0%

---

# 데이터 세트 규칙

데이터 세트 규칙은 조화 된 필드를 Mix Modeler에서 수집한 데이터의 필드와 매핑하는 데 도움이 됩니다.

* Adobe Experience Platform에서 수집한 집계 데이터의 경우 사용 가능한 데이터 세트 필드 중 하나 이상을 적절한 조화된 필드에 매핑합니다.
* 이벤트 데이터의 경우, 직접 또는 조건을 사용하여 하나 이상의 조정된 필드를 데이터 세트의 필드에 개별적으로 매핑할 수 있습니다.


## 데이터 세트 규칙 관리

사용 가능한 데이터 세트 규칙의 표를 보려면 Mix Modeler 인터페이스에서 다음을 수행하십시오.

1. 선택 ![데이터 검색](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** 왼쪽 레일에서.

1. 선택 **[!UICONTROL Dataset rules]** 을 클릭합니다. 데이터 세트 규칙 표가 표시됩니다.

테이블 열은 데이터 세트 규칙에 대한 세부 사항을 지정합니다.

| 열 이름 | 세부 사항 |
| ---------------------- | ----------|
| 데이터 세트 | 데이터 세트의 이름입니다. |
| 소스 | Adobe Analytics, 경험 이벤트, 요약(집계) 또는 소비자 경험 이벤트일 수 있는 데이터 세트의 소스. |
| 스키마 | 데이터 세트가 준수하는 스키마. 스키마 이름을 빠르게 선택하여 Mix Modeler - 스키마의 스키마 편집기의 새 탭에서 스키마를 열 수 있습니다. |
| 세부기간 | 데이터 집합에 있는 데이터의 세부기간입니다. 가능한 값은 일별, 주별, 월별 또는 연도별입니다. |
| 주의 시작 | 특정 데이터 세트에 대해 새 주의 시작으로 간주되는 요일을 지정합니다. |
| 상태 | 필드의 상태: <p><span style="color:gray">●</span> 초안 또는 <p><span style="color:green">●</span> 활성 |
| 마지막 수정일 | 데이터 집합 규칙을 마지막으로 수정한 데이터 및 시간입니다. |

{style="table-layout:auto"}

### 데이터 세트 규칙 만들기

데이터 세트 규칙을 만들려면 ![데이터 검색](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Dataset rules]** Mix Modeler에서 인터페이스, 선택 **[!UICONTROL Create Dataset rule]** 다음에서 **[!UICONTROL Dataset rules configuration]** 마법사.

다음에서 **[!UICONTROL Create]** 화면,

1. 위치 **[!UICONTROL Dataset details]**, 데이터 세트 선택 **[!UICONTROL Select dataset]** 구성을 시작합니다. 목록에서 데이터 세트는 다음과 같이 분류됩니다 **[!UICONTROL Consumer Experience Events]**, **[!UICONTROL Adobe Analytics]**, **[!UICONTROL Experience Event]** 및 **[!UICONTROL Summary]**.

1. 에 대한 날짜 선택 **[!UICONTROL Start of the week]**.

1. 선택 **[!UICONTROL Daily]**, **[!UICONTROL Weekly]**, **[!UICONTROL Monthly]** 또는 **[!UICONTROL Yearly]** 대상 **[!UICONTROL Granularity]**.

1. 다음의 데이터 세트를 선택한 경우 **[!UICONTROL Summary]** 범주:

   1. 각 를 매핑합니다. **[!UICONTROL Available dataset fields]** 해당 항목에 **[!UICONTROL Standard harmonized fields]** 위치: **[!UICONTROL Map to harmonized fields]**. 데이터 세트 필드를 조정된 필드에 매핑하지 않으려면 을(를) 명시적으로 선택합니다. **[!UICONTROL -- None --]**.

   1. 목록에서 사용할 수 없는 새 조화로운 필드가 필요한 경우 다음을 선택합니다. **[!UICONTROL Create New]** 새로운 조화로운 필드를 만들 수 있습니다. 대화 상자에 요약되어 있습니다. [새 조화로운 필드 추가](fields.md#add-a-harmonized-field) 을 사용하면 새로운 조화로운 필드를 빠르게 추가할 수 있습니다.

   1. 규칙의 모든 필드에 대한 매핑이 완료되면 다음을 선택합니다. **[!UICONTROL Save as draft]** 규칙의 초안 버전 저장하기 또는 **[!UICONTROL Save]** 을 클릭하여 규칙을 저장하고 활성화합니다.  선택 **[!UICONTROL Cancel]** 규칙 구성을 취소합니다.

      ![데이터 세트 규칙 만들기](../assets/dataset-create-summary.png)

1. 이벤트 범주 데이터 세트를 선택한 경우(**[!UICONTROL Experience Events]**, **[!UICONTROL Adobe Analytics]**, **[!UICONTROL Consumer Experience Events]**), 아래 상자에서 **[!UICONTROL Map to harmonized fields]**:

   1. 다음 위치에서 조화로운 필드 선택 **[!UICONTROL Standard harmonized field]**.

   1. 선택한 조화로운 필드가 유형 지표인 경우:

      1. 선택 **[!UICONTROL Count]** 또는 **[!UICONTROL Sum]** 출처: **[!UICONTROL Mapping type]**.

      1. 선택 **[!UICONTROL *AEP 데이터 세트 필드&#x200B;*]**기본적으로 harmonized 필드가 매핑되도록 합니다.

   1. 선택한 필드가 차원 유형인 경우:

      1. 선택 **[!UICONTROL Map Into]** 또는 **[!UICONTROL Case]** 출처: **[!UICONTROL Mapping type]**.

      1. 다음을 선택한 경우 **[!UICONTROL Map Into]**, 선택 **[!UICONTROL Field]** 및 **[!UICONTROL *AEP 데이터 세트 필드&#x200B;*]**또는&#x200B;**[!UICONTROL Value]**및 기본값이 설정되어 있는 필드를 데이터 세트 필드 또는 입력된 값에 매핑합니다.

      1. 다음을 선택한 경우 **[!UICONTROL Case]**, 선택 **[!UICONTROL Field]** 및 **[!UICONTROL *AEP 데이터 세트 필드&#x200B;*]**또는&#x200B;**[!UICONTROL Value]**및 기본값이 설정되어 있는 필드를 데이터 세트 필드 또는 입력된 값에 매핑합니다.

         1. 또한 값을 명시적으로 설정하는 하나 이상의 조건으로 구성된 하나 이상의 사례를 정의합니다. 각 조건은 특정 항목을 확인할 수 있습니다 **[!UICONTROL *AEP 데이터 세트 필드&#x200B;*]**해당 여부&#x200B;**[!UICONTROL Exists]**또는&#x200B;**[!UICONTROL Not Exists]**아님&#x200B;**[!UICONTROL Contains]**,**[!UICONTROL Not Contains]**,**[!UICONTROL Equals]**,**[!UICONTROL Not Equals]**,**[!UICONTROL Starts With]**, 또는&#x200B;**[!UICONTROL Ends With]**다음 위치에 입력된 값**[!UICONTROL *&#x200B;입력 값 입력&#x200B;*]**.

         1. 다른 서비스 케이스를 추가하려면 다음을 선택합니다. ![추가](../assets/icons/AddCircle.svg) **[!UICONTROL Add case]**&#x200B;를 클릭하여 다른 조건을 추가합니다. ![추가](../assets/icons/AddCircle.svg) **[!UICONTROL Add condition]**.

         1. 대/소문자 또는 조건을 삭제하려면 ![닫기](../assets/icons/Close.svg) 를 입력합니다.

         1. 서비스 케이스에 조건을 적용할지 또는 모두 적용할지를 선택하려면 다음을 선택합니다. **[!UICONTROL Any of]** 또는 **[!UICONTROL All of]**.

         1. 사례에 대한 결과 값을 설정하려면 다음 값을 입력합니다. **[!UICONTROL Then]**.

      아래 예

      * 를 사용합니다. **[!UICONTROL Map Into]** **[!UICONTROL Mapping type]** 를 매핑하려면 다음을 수행하십시오. **[!UICONTROL Channel Type At Source]** 이(가) (으)로 조화된 필드 **[!UICONTROL channel_type]** 의 필드 **[!DNL Luma Transactions]** 데이터 세트.

      * 를 사용합니다. **[!UICONTROL Case]** **[!UICONTROL Mapping type]** 의 값을 조건부로 매핑하려면 **[!UICONTROL marketing.campaignName]** 의 필드 **[!DNL Luma Transactions]** 데이터 세트를 **[!UICONTROL Campaign]** 조화로운 필드. Campaign harmonized 필드가 다음으로 설정됨:

         * `Black Friday` 다음과 같은 경우 **[!UICONTROL marketing.campaignName]** 은(는) `_black_friday` 또는 `BlackFriday`.
         * 을(를) 의 값으로 **[!UICONTROL marketing.campaignName]** 다른 모든 경우에.

        ![데이터 세트 규칙 이벤트](../assets/dataset-create-event.png)

1. 선택 ![추가](../assets/icons/AddCircle.svg) **[!UICONTROL Add field]** 추가 필드를 정의합니다.

완료되면 다음을 선택합니다. **[!UICONTROL Save as draft]** 규칙의 초안 버전 저장하기 또는 **[!UICONTROL Save]** 을 클릭하여 규칙을 저장하고 활성화합니다.  선택 **[!UICONTROL Cancel]** 규칙 구성을 취소합니다.


### 데이터 세트 규칙 편집

데이터 세트 규칙을 편집하려면 ![데이터 검색](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Dataset rules]** Mix Modeler 인터페이스:

1. 선택 ![자세히](../assets/icons/More.svg) 다음에서 **[!UICONTROL Dataset]** 편집할 데이터 세트 규칙에 대한 열입니다.
1. 컨텍스트 메뉴에서 을(를) 선택합니다 ![편집](../assets/icons/Edit.svg) **[!UICONTROL Edit]** 데이터 세트 규칙 편집을 시작합니다. 을(를) 참조하십시오 [데이터 세트 규칙 만들기](#create-a-dataset-rule) 을 참조하십시오.


### 데이터 세트 규칙 삭제

데이터 세트 규칙을 삭제하려면 ![데이터 검색](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Dataset rules]** Mix Modeler 인터페이스:

1. 선택 ![자세히](../assets/icons/More.svg) 다음에서 **[!UICONTROL Dataset]** 삭제할 데이터 세트 규칙에 대한 열입니다.
1. 컨텍스트 메뉴에서 을(를) 선택합니다 ![삭제](../assets/icons/Delete.svg) **[!UICONTROL Delete]** 데이터 세트 규칙을 삭제합니다. 확인을 묻는 메시지가 표시됩니다. 선택 **[!UICONTROL Delete]** 선택한 데이터 세트 규칙을 영구적으로 삭제하려면 다음 작업을 수행하십시오.


## 데이터 동기화

통합 데이터와 요약 및/또는 이벤트 데이터 세트 간에 데이터를 동기화하려면 데이터 세트 규칙의 모든 논리를 따르십시오.

1. **[!UICONTROL Sync data]**&#x200B;를 선택합니다.

1. 다음에서 **[!UICONTROL Sync data for dataset rules]** 대화 상자에서 다음 중 하나를 선택합니다 **[!UICONTROL Refresh harmonized data for summary datasets]**, **[!UICONTROL Refresh harmonized data for event datasets]**, 또는 **[!UICONTROL Refresh harmonized data for both summary + event datasets]**.

1. 선택 **[!UICONTROL Sync]** 데이터 세트에 있는 데이터와 조정된 데이터 간에 정의된 데이터 세트 규칙을 기반으로 동기화를 시작합니다. 동기화를 취소하려면 다음을 선택합니다 **[!UICONTROL Cancel]**.

   ![데이터 동기화](../assets/sync-data.png)


## 데이터 병합 환경 설정

요약된 데이터와 이벤트 소스의 데이터가 함께 병합될 때 충돌을 해결하기 위한 환경 설정을 정의할 수 있습니다. 방법은 다음과 같습니다.

1. 선택 ![데이터 병합 환경 설정](../assets/icons/Merge.svg) **데이터 병합 환경 설정**.

1. 다음에서 **[!UICONTROL Data merge preferences]** 대화 상자:

   ![데이터 병합 환경 설정](../assets/data-merge-preferences.png)

   1. 에서 기본 지표 환경 설정 선택 **[!UICONTROL Default metric preference]** 목록을 표시합니다. <p>조화 중에 여러 데이터 소스가 지정된 채널에 대한 지표 필드를 업데이트하려고 하면 기본 환경 설정이 적용됩니다. 이 환경 설정은에 정의된 특정 지표 환경 설정에 대해 재정의되지 않는 한 샌드박스 수준에서 적용됩니다. **[!UICONTROL Metric based preference]**.

   1. 사용 ![플러스](../assets/icons/AddCircle.svg) **[!UICONTROL Add a metric]**, 하나 이상의 지표를 아래에 추가 **[!UICONTROL Metric based preference]**.



      * 다음에서 지표 선택 **[!UICONTROL _지표 선택_]** 목록 및
      * **[!UICONTROL Summary]** 또는&#x200B;**[!UICONTROL Event]**&#x200B;를 선택합니다.

      사용 ![삭제](../assets/icons/Close.svg) 목록에서 항목을 삭제합니다.

   1. 선택 **[!UICONTROL Save]** 데이터 병합 환경 설정을 저장합니다. 선택 **[!UICONTROL Cancel]** 취소합니다.
