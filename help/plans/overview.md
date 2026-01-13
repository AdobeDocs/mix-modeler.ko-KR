---
title: 플랜 개요
description: Mix Modeler에서 플랜을 보고, 선택하고, 실행하는 방법을 알아봅니다.
feature: Plans
exl-id: 45a8dc30-3259-493d-8ea5-1899903733a6
source-git-commit: 0d11168b71319e6c854482f89dbb1bb68962a880
workflow-type: tm+mt
source-wordcount: '698'
ht-degree: 0%

---

# 플랜 개요

Mix Modeler의 플랜을 사용하면 비즈니스 단위 및 채널별로 예산을 할당할 수 있습니다. 계획 기능은 조정된 데이터를 기반으로 훈련된 모델의 결과와 통합되어 있습니다.

이 계획에서는 주어진 기간 동안 마케팅 관련 프로젝트에 소비하려는 재량적 투자(예: 예산)에 대해 간략히 설명합니다. 이러한 투자는 일반적인 KPI(예: 주문, 매출)를 활용합니다. 플랜에는 유료 광고, 스폰서 웹 콘텐츠, 이벤트 등의 채널 비용이 포함될 수 있습니다.

플랜에는 다음이 필요합니다.

- 모델,
- 데이터 범위,
- 예산.

제도는 다음을 선택적으로 포함할 수 있습니다.

- 구성된 인식 창,
- 각각에 타겟 예산이 있는 여러 플라이트 날짜
- 채널 및 플라이트 일자별 최소 및 최대 예산 제한.

플랜에 사용한 모델이 새 데이터에서 점수가 매겨지는 경우, 점수가 다시 매겨진 데이터를 고려하여 새 플랜을 만들어야 합니다.


## 계획 수립

계획을 수립하려면 Mix Modeler 계획 생성 마법사를 사용하십시오. 자세한 내용은 [계획 수립](build.md)을 참조하세요.


## 계획 관리

Mix Modeler 인터페이스에서 현재 계획의 테이블을 보려면 다음을 수행합니다.

1. 왼쪽 레일에서 ![](/help/assets/icons2/FileChart.svg) **[!UICONTROL Plans]**&#x200B;을(를) 선택합니다.

1. 현재 플랜과 해당 상태에 대한 표가 표시됩니다.

   테이블 열은 계획에 대한 세부 사항을 지정합니다.

   | 열 이름 | 세부 사항 |
   |---|---|
   | 이름 | 플랜 이름 |
   | 모델 | 계획의 기반으로 사용되는 모델입니다. |
   | 날짜 범위 | 플랜에 대한 전체 날짜 범위입니다. |
   | 예산 | 플랜에 대한 총 예산. |
   | 계획 대상 | 대상 기반 계획에 대해 정의된 대상 지표. |
   | 예측 반환 | 플랜에 대한 [예측된 반환](/help/main-guide/glossary.md) |
   | 예측된 ROI | 플랜에 대한 [예측된 ROI](/help/main-guide/glossary.md). |
   | 예측 전환 | 플랜에 대한 [예측된 전환](/help/main-guide/glossary.md) |
   | 예측된 CPA | 플랜에 대한 [예측된 CPA](/help/main-guide/glossary.md) |
   | 상태 | 플랜 상태: <p><span style="color:red">●</span> 실패, <p><span style="color:blue">●</span> 처리 중 또는 <p><span style="color:green">●</span>이(가) 완료되었습니다. |

   {style="table-layout:auto"}

   ![ColumnSetting](/help/assets/icons/ColumnSetting.svg)을(를) 사용하여 테이블에 표시할 열을 ![확인 표시](/help/assets/icons/Checkmark.svg)할 수 있습니다.

   오름차순 ![ArrowMoveUp](/help/assets/icons2/ArrowMoveUp.svg) 또는 내림차순 ![ArrowMoveDown](/help/assets/icons2/ArrowMoveDown.svg)순서로 열의 테이블을 정렬하려면 열의 제목을 선택합니다.

   **[!UICONTROL Name]**, **[!UICONTROL Model]** 또는 **[!UICONTROL Date range]** 열을 정렬하거나 크기를 조정하려면 **[!UICONTROL Name]** ![V자형 화살표](/help/assets/icons/ChevronDown.svg), **[!UICONTROL Model]** ![V자형 화살표](/help/assets/icons/ChevronDown.svg) 또는 **[!UICONTROL Date range]** ![V자형 화살표](/help/assets/icons/ChevronDown.svg)를 선택하십시오. 컨텍스트 메뉴에서 **[!UICONTROL Sort ascending]**, **[!UICONTROL Sort descending]** 또는 **[!UICONTROL Resize column]**&#x200B;을(를) 선택합니다. 또는 이러한 열의 열 구분자 위로 마우스를 가져가 열 크기를 조정할 수 있습니다.

1. ![검색](/help/assets/icons/Search.svg)을 사용하여 하나 이상의 특정 계획에 대한 테이블을 검색하고 필터링합니다.

### 플랜 인사이트

계획의 통찰력을 조회하고 계획을 편집하려면

1. 왼쪽 레일에서 ![PLan](/help/assets/icons/FileChart.svg) **[!UICONTROL Plans]**&#x200B;을(를) 선택합니다.

1. 계획명을 선택합니다.

[플랜 인사이트](insights.md)(으)로 리디렉션되었습니다.


### 플랜 복제

계획을 복제하려면

- 플랜에 대해 ![자세히](/help/assets/icons/More.svg)을(를) 선택하십시오. 컨텍스트 메뉴에서 **[!UICONTROL Duplicate]**&#x200B;을(를) 선택합니다.
- 또는 ![SelectBox](/help/assets/icons/SelectBox.svg) 테이블에서 플랜을 선택하고 파란색 작업 표시줄에서 ![복사](/help/assets/icons/Copy.svg) **[!UICONTROL Duplicate]**&#x200B;을(를) 선택합니다.

원래 계획 이름에 **[!UICONTROL (Copy)] (_n_)**&#x200B;을(를) 추가한 이름으로 구성된 새 계획이 만들어집니다. 복사된 플랜에 대한 업데이트된 세부 정보를 제공하기 위해 [플랜 만들기](build.md)(으)로 자동으로 리디렉션됩니다.

- 최초 계획의 상세내역(예: 설명, 예산 등)이 복사됩니다.
- 최초 계획의 예산 제한조건이 새로 생성된 계획에 복사됩니다.
- 복사된 계획의 기반으로 다른 모델을 선택할 수 있는 옵션이 있습니다.
   - 복사된 계획에는 존재하지만 새로 선택된 모델에는 존재하지 않는 접점 또는 채널의 경우, 이러한 접점 또는 채널에 대한 모든 제한이 계획에서 제거됩니다.
   - 복사된 계획에는 존재하지 않지만 새로 선택된 모델에는 존재하는 접점 또는 채널의 경우 제한은 다음과 같이 설정됩니다.
      - 최소값은 `0`이고,
      - 계획 플라이트 범위 예산에 따른 최대값입니다.



### 계획 비교

계획을 비교하려면

1. 테이블에서 두 개의 계획을 선택합니다.
1. 파란색 작업 표시줄에서 ![비교](/help/assets/icons/Compare.svg) **[!UICONTROL Compare]**&#x200B;을(를) 선택합니다. **[!UICONTROL Compare plans]** UI가 표시됩니다.


### 계획 삭제

계획을 삭제하려면

1. 플랜에 대해 ![자세히](/help/assets/icons/More.svg)을(를) 선택하십시오. 컨텍스트 메뉴에서 **[!UICONTROL Delete]**&#x200B;을(를) 선택합니다. <br/>또는 ![SelectBox](/help/assets/icons/SelectBox.svg) 테이블에서 계획을 선택하고 파란색 작업 표시줄에서 ![삭제](/help/assets/icons/Delete.svg) **[!UICONTROL Delete]**&#x200B;을(를) 선택합니다.
1. **[!UICONTROL Delete]** 확인 대화 상자에서 **[!UICONTROL Delete plan]**&#x200B;을(를) 선택하여 계획을 삭제합니다. 취소할 **[!UICONTROL Cancel]**&#x200B;을(를) 선택하십시오.

복수 계획을 삭제하려면

1. 여러 계획을 선택합니다.
1. 파란색 작업 표시줄에서 ![삭제](/help/assets/icons/Delete.svg) **[!UICONTROL Delete]**&#x200B;을(를) 선택하여 계획을 삭제합니다.
1. **[!UICONTROL Delete]** x **[!UICONTROL Delete *계획&#x200B;*확인 대화 상자에서]**&#x200B;을(를) 선택하여 계획을 삭제합니다. 취소할&#x200B;**[!UICONTROL Cancel]**&#x200B;을(를) 선택하십시오.


