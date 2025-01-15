---
title: 플랜
description: Mix Modeler에서 플랜을 보고, 선택하고, 실행하는 방법을 알아봅니다.
feature: Plans
exl-id: 45a8dc30-3259-493d-8ea5-1899903733a6
source-git-commit: 0475c584b3963d02d9dd72f0dccf692d558463db
workflow-type: tm+mt
source-wordcount: '539'
ht-degree: 0%

---

# 플랜

Mix Modeler의 플랜을 사용하면 비즈니스 단위 및 채널별로 예산을 할당할 수 있습니다. 계획 기능은 조정된 데이터를 기반으로 훈련된 모델의 결과와 통합되어 있습니다.

플랜에서는 공통 KPI(예: 주문, 매출)를 사용하여 주어진 기간 동안 마케팅 관련 프로젝트에 소비하려는 재량적 투자(예: 예산)에 대해 간략히 설명합니다. 요금제에는 유료 광고, 후원한 웹 콘텐츠, 이벤트 등의 채널 비용이 포함될 수 있습니다.

플랜에는 다음이 필요합니다.

- 모델,
- 데이터 범위,
- 예산.

제도는 다음을 선택적으로 포함할 수 있습니다.

- 구성된 인식 창,
- 각각에 타겟 예산이 있는 여러 플라이트 날짜
- 채널 및 플라이트 일자별 최소 및 최대 예산 제한.


## 계획 관리

Mix Modeler 인터페이스에서 현재 계획의 테이블을 보려면 다음을 수행합니다.

1. 왼쪽 레일에서 ![](/help/assets/icons/FileChart.svg) **[!UICONTROL Plans]**&#x200B;을(를) 선택합니다.

1. 현재 플랜과 해당 상태에 대한 표가 표시됩니다.

   테이블 열은 계획에 대한 세부 사항을 지정합니다.

   | 열 이름 | 세부 사항 |
   |---|---|
   | 이름 | 플랜 이름 |
   | 모델 | 계획의 기반으로 사용되는 모델입니다. |
   | 날짜 범위 | 플랜에 대한 전체 날짜 범위입니다. |
   | 예산 | 플랜에 대한 총 예산. |
   | 예측 반환 | 플랜에 대한 예측 반환 |
   | 예측된 ROI | 플랜에 대한 예측된 ROI. |
   | 예측 전환 | 플랜에 대한 예측된 전환 |
   | 예측된 CPA | 플랜에 대한 예측된 CPA |
   | 상태 | 플랜 상태: <p><span style="color:red">●</span> 실패, <p><span style="color:blue">●</span> 처리 중, 또는 <p><span style="color:green">●</span>이(가) 완료되었습니다. |

   {style="table-layout:auto"}

   ![ColumnSetting](/help/assets/icons/ColumnSetting.svg)을(를) 사용하여 테이블에 표시할 열을 ![확인 표시](/help/assets/icons/Checkmark.svg)할 수 있습니다.

1. ![검색](/help/assets/icons/Search.svg)을 사용하여 하나 이상의 특정 계획에 대한 테이블을 검색하고 필터링합니다.

## 계획 만들기

계획을 생성하려면 Mix Modeler 계획 생성 마법사를 사용합니다. 자세한 내용은 [계획 만들기](create.md)를 참조하십시오.


## 플랜 편집

계획을 편집하려면 테이블에서 계획명을 선택합니다. 자세한 내용은 [플랜 편집](edit.md)을 참조하십시오.


## 플랜에 대한 선택 및 조치

하나 이상의 플랜을 선택할 수 있으며, 이렇게 하면 플랜 작업 표시줄이 표시됩니다. 작업 표시줄을 사용하여 계획을 삭제, 비교 또는 복제할 수 있습니다.

계획 테이블에서 모든 선택 항목을 제거하려면 작업 표시줄에서 ![닫기](/help/assets/icons/Close.svg)를 선택합니다

![플랜 작업 표시줄](/help/assets/plans-action-bar.png)

### 플랜 복제

계획을 복제하려면

1. 테이블에서 단일 계획을 선택합니다.
1. 작업 표시줄에서 ![복사](/help/assets/icons/Copy.svg) **[!UICONTROL Duplicate]**&#x200B;을(를) 선택합니다. 원래 계획 이름에 **[!UICONTROL (Copy)]**&#x200B;을(를) 추가한 새 계획이 테이블 맨 위에 추가됩니다.

또는

1. 테이블의 플랜에 대해 ![자세히](/help/assets/icons/More.svg)을(를) 선택하십시오.
1. 상황에 맞는 메뉴에서 **[!UICONTROL Duplicate]**&#x200B;을(를) 선택합니다. 원래 계획 이름에 **[!UICONTROL (Copy)]**&#x200B;을(를) 추가한 새 계획이 테이블 맨 위에 추가됩니다.

### 계획 비교

계획을 비교하려면

1. 테이블에서 두 개의 계획을 선택합니다.
1. 작업 표시줄에서 ![비교](/help/assets/icons/Compare.svg) **[!UICONTROL Compare]**&#x200B;을(를) 선택합니다. **[!UICONTROL Compare plans]** UI가 표시됩니다.


### 계획 삭제

계획을 삭제하려면

1. 왼쪽 레일에서 ![](/help/assets/icons/FileChart.svg) **[!UICONTROL Plans]**&#x200B;을(를) 선택합니다.
1. 플랜에 대해 ![자세히](/help/assets/icons/More.svg)를 선택하고 상황에 맞는 메뉴에서 **[!UICONTROL Delete]**&#x200B;을(를) 선택합니다. 또는 파란색 작업 표시줄에서 ![삭제](/help/assets/icons/Delete.svg) **[!UICONTROL Delete]**&#x200B;을(를) 선택합니다.
1. **[!UICONTROL Delete moplandel]** 확인 대화 상자에서 **[!UICONTROL Delete]**&#x200B;을(를) 선택하여 계획을 삭제합니다. 취소할 **[!UICONTROL Cancel]**&#x200B;을(를) 선택하십시오.

복수 계획을 삭제하려면

1. 여러 계획을 선택합니다.
1. 파란색 작업 표시줄에서 ![삭제](/help/assets/icons/Delete.svg) **[!UICONTROL Delete]**&#x200B;을(를) 선택하여 계획을 삭제합니다.
1. **[!UICONTROL Delete *x *계획]**확인 대화 상자에서&#x200B;**[!UICONTROL Delete]**을(를) 선택하여 계획을 삭제합니다. 취소할&#x200B;**[!UICONTROL Cancel]**을(를) 선택하십시오.
