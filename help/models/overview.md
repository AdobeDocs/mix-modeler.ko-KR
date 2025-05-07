---
title: 모델 개요
description: Mix Modeler에서 모델을 구축하고 사용하는 방법에 대해 알아봅니다.
feature: Models
exl-id: c43d9bc9-4429-45c2-9247-bd24510a24be
source-git-commit: 6855d19347b7f6f1477a6265310df5950b8463c9
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 0%

---

# 모델 개요

Mix Modeler의 모델 기능을 사용하면 비즈니스 목표에 맞는 모델을 구성하고, 교육하고, 평가할 수 있습니다. 교육 및 점수는 멀티터치 기여도 분석과 마케팅 믹스 모델링 간의 AI 기반 전환 학습을 지원합니다.

이 모델은 Mix Modeler 애플리케이션 워크플로의 일부로 만드는 통합 데이터를 기반으로 합니다.

Mix Modeler의 모델은 마케터의 투자를 기반으로 지정된 결과를 측정하고 예측하기 위해 사용되는 머신 러닝 모델입니다. 마케팅 접점 및 요약 수준 데이터를 입력으로 사용할 수 있습니다. Mix Modeler을 사용하면 매출, 판매 수량, 리드 등과 같은 다양한 변수, 차원 및 결과 세트를 기반으로 모델의 변형을 만들 수 있습니다.

모델은 다음을 필요로 합니다.

* 전환 1개.
* 요약 수준 데이터, 마케팅 접점 데이터(이벤트 데이터) 또는 둘 다로 구성된 하나 이상의 마케팅 접점(채널).
* 구성 가능한 전환 확인 기간.
* 구성 가능한 교육 창.

모델은 다음을 선택적으로 포함할 수 있습니다.

* 외부 요인.
* 내부 요인.
* 과거 관련자 경험, 증분 테스트, 기타 모델 등 다른 소스의 마케팅 기여에 대한 사전 지식.
* 마케팅 데이터가 희소할 때 상대 지출 공유를 프록시로 사용하는 지출 공유.

모형을 처음 만들었을 때, 그 만들기는 곧바로 훈련과 채점 과정을 시작한다. 초기 교육 및 채점 실행이 완료되면 모델 인사이트를 검토할 수 있습니다. 모델은 이후 재학습될 수 있습니다. 또한 모델을 수동으로 다시 검색해야 하는 모델에 데이터를 추가할 수 있습니다. 재교육 및 재채점은 비즈니스 목표에 가장 적합한 모델 적합성을 얻기 위해 새로운 발견과 정보가 나타나고 조정이 필요하므로 반복적인 프로세스입니다.


## 모델 구축

모델을 만들려면 **[!UICONTROL Open model canvas]**&#x200B;을(를) 선택할 때 사용할 수 있는 Mix Modeler 단계별 안내식 모델 구성 흐름을 사용하십시오. 자세한 내용은 [모델 빌드](build.md)를 참조하십시오.

## 모델 관리

Mix Modeler 인터페이스에서 현재 모델의 표를 보려면 다음을 수행하십시오.

1. 왼쪽 레일에서 ![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]**&#x200B;을(를) 선택합니다.

1. 현재 모델의 표가 표시됩니다.

   테이블 열은 모델에 대한 세부 사항을 지정합니다.

   | 열 이름 | 세부 사항 |
   |---|---|
   | 이름 | 모델 이름 |
   | 설명 | 모델에 대한 설명 |
   | 전환 이벤트 | 모델에 대해 선택한 변환입니다. |
   | 실행 빈도 | 모델 교육의 실행 빈도입니다. |
   | 마지막 실행 | 모델의 마지막 교육 날짜 및 시간입니다. |
   | 상태 | 모델의 상태입니다. |

   {style="table-layout:auto"}

   모델의 보고된 상태는 모델이 라이프사이클 내에 있는 위치에 따라 다릅니다. 예를 들어 모델이 생성되었는지, (재)트레이닝이 성공했는지 또는 (재)채점이 성공했는지 여부에 상관없이 표시됩니다.

   아래 표에서:

   * ![확인 표시](/help/assets/icons/Checkmark.svg) - 모델 라이프사이클에서 단계가 성공적으로 실행되었음을 나타냅니다.
   * ![시계](/help/assets/icons/Clock.svg) - 모델 수명 주기에서 현재 진행 중인 단계 실행을 나타냅니다.
   * ![닫기](/help/assets/icons/Close.svg) - 모델 수명 주기에서 단계 실행이 실패했음을 나타냅니다.

   | 상태 | [빌드](/help/models/build.md) | [교육](/help/models/train-score.md#train) | [점수](/help/models/train-score.md#score) | [다시 교육](/help/models/train-score.md#train) | [다시 검색](/help/models/train-score.md#score) |
   |---|:---:|:---:|:---:|:---:|:---:|
   | 진행 중 | ![확인 표시](/help/assets/icons/Checkmark.svg) | | | | |
   | 진행 중 | ![확인 표시](/help/assets/icons/Checkmark.svg) | ![시계](/help/assets/icons/Clock.svg) | | | |
   | 진행 중 | ![확인 표시](/help/assets/icons/Checkmark.svg) | ![확인 표시](/help/assets/icons/Checkmark.svg) | ![시계](/help/assets/icons/Clock.svg) | | |
   | 진행 중 | ![확인 표시](/help/assets/icons/Checkmark.svg) | ![확인 표시](/help/assets/icons/Checkmark.svg) | ![확인 표시](/help/assets/icons/Checkmark.svg) | ![시계](/help/assets/icons/Clock.svg) | |
   | 진행 중 | ![확인 표시](/help/assets/icons/Checkmark.svg) | ![확인 표시](/help/assets/icons/Checkmark.svg) | ![확인 표시](/help/assets/icons/Checkmark.svg) | ![확인 표시](/help/assets/icons/Checkmark.svg) | ![시계](/help/assets/icons/Clock.svg) |
   | 교육 실패 | ![확인 표시](/help/assets/icons/Checkmark.svg) | ![닫기](/help/assets/icons/Close.svg) | | | |
   | 교육 실패 | ![확인 표시](/help/assets/icons/Checkmark.svg) | ![확인 표시](/help/assets/icons/Checkmark.svg) | ![확인 표시](/help/assets/icons/Checkmark.svg) | ![닫기](/help/assets/icons/Close.svg) | |
   | 교육 성공 | ![확인 표시](/help/assets/icons/Checkmark.svg) | ![확인 표시](/help/assets/icons/Checkmark.svg) | | | |
   | 교육 성공 | ![확인 표시](/help/assets/icons/Checkmark.svg) | ![확인 표시](/help/assets/icons/Checkmark.svg) | ![확인 표시](/help/assets/icons/Checkmark.svg) | ![확인 표시](/help/assets/icons/Checkmark.svg) | |
   | 채점 실패 | ![확인 표시](/help/assets/icons/Checkmark.svg) | ![확인 표시](/help/assets/icons/Checkmark.svg) | ![닫기](/help/assets/icons/Close.svg) | | |
   | 채점 실패 | ![확인 표시](/help/assets/icons/Checkmark.svg) | ![확인 표시](/help/assets/icons/Checkmark.svg) | ![확인 표시](/help/assets/icons/Checkmark.svg) | ![확인 표시](/help/assets/icons/Checkmark.svg) | ![닫기](/help/assets/icons/Close.svg) |
   | 채점 성공 | ![확인 표시](/help/assets/icons/Checkmark.svg) | ![확인 표시](/help/assets/icons/Checkmark.svg) | ![확인 표시](/help/assets/icons/Checkmark.svg) | | |
   | 채점 성공 | ![확인 표시](/help/assets/icons/Checkmark.svg) | ![확인 표시](/help/assets/icons/Checkmark.svg) | ![확인 표시](/help/assets/icons/Checkmark.svg) | ![확인 표시](/help/assets/icons/Checkmark.svg) | ![확인 표시](/help/assets/icons/Checkmark.svg) |

   {style="table-layout:fixed"}

1. 목록에 표시되는 열을 변경하려면 ![열 설정](/help/assets/icons/ColumnSetting.svg)을 선택하고 ![확인](/help/assets/icons/Checkmark.svg)을 설정하거나 해제합니다.

특정 모델에 대해 다음 작업을 수행할 수 있습니다.

### 모델 인사이트

모델 인사이트 기능은 성공적으로 교육되고 채점된 모델에서만 사용할 수 있습니다.

모델의 통찰력을 보려면 다음 작업을 수행하십시오.

1. 왼쪽 레일에서 ![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]**&#x200B;을(를) 선택합니다.

1. 모델 이름을 선택합니다.

[모델 인사이트](insights.md)(으)로 리디렉션되었습니다.


### 세부 정보 보기

모델의 세부 정보를 보려면 다음 작업을 수행하십시오.

1. 왼쪽 레일에서 ![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]**&#x200B;을(를) 선택합니다.

1. 세부 정보가 포함된 팝업을 표시하려면 모델에 대한 ![정보](/help/assets/icons/Info.svg)을(를) 선택하십시오.


### 복제

모델을 빠르게 복제할 수 있습니다.

1. 왼쪽 레일에서 ![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]**&#x200B;을(를) 선택합니다.

1. 모델에 대해 ![자세히](/help/assets/icons/More.svg)를 선택하고 상황에 맞는 메뉴에서 **[!UICONTROL Duplicate]**&#x200B;을(를) 선택합니다.

원래 모델 이름에 **[!UICONTROL (Copy)](_n_)**&#x200B;이(가) 추가된 제안된 이름으로 새 모델을 만드는 단계로 리디렉션됩니다.

### 편집

모델의 이름, 설명 및 교육 및 채점 일정을 편집할 수 있습니다.

1. 왼쪽 레일에서 ![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]**&#x200B;을(를) 선택합니다.

1. 모델에 대해 ![자세히](/help/assets/icons/More.svg)를 선택하고 상황에 맞는 메뉴에서 **[!UICONTROL Edit]**&#x200B;을(를) 선택합니다.

   **[!UICONTROL Edit model]** 대화 상자에서:

   * 새 **[!UICONTROL Name]** 및 **[!UICONTROL Description]**&#x200B;을(를) 입력하십시오.

   * 예약을 사용하려면 **[!UICONTROL Status]**&#x200B;을(를) 사용하도록 설정하십시오. 교육되고 점수가 매겨진 모델만 예약할 수 있습니다.

      1. **[!UICONTROL Scoring frequency]** 선택:

         * **[!UICONTROL Daily]**: 올바른 시간(예: `05:22 pm`)을 입력하거나 ![시계](/help/assets/icons/Clock.svg)를 사용하십시오.
         * **[!UICONTROL Weekly]**: 요일을 선택하고 올바른 시간(예: `05:22 pm`)을 입력하거나 ![시계](/help/assets/icons/Clock.svg)를 사용하십시오.
         * **[!UICONTROL Monthly]**: 모든 드롭다운 메뉴에서 요일을 선택하고 올바른 시간(예: `05:22 pm`)을 입력하거나 ![시계](/help/assets/icons/Clock.svg)를 사용하십시오.

      1. 드롭다운 메뉴에서 **[!UICONTROL Training frequency]**&#x200B;을(를) 선택합니다. **[!UICONTROL Monthly]**, **[!UICONTROL Quarterly]**, **[!UICONTROL Yearly]** 또는 **[!UICONTROL None]**.

     ![모델 편집](../assets/model-edit.png)

1. **[!UICONTROL Save]**&#x200B;를 선택합니다.



### 교육

새로운 증분 마케팅 및 요소 데이터를 포함하려는 경우 모델을 다시 교육하는 것이 좋습니다. 자세한 내용은 [모델 교육 및 점수](train-score.md#train)를 참조하십시오.


### 점수

새 마케팅 데이터를 기반으로 모델에 증분 점수를 매기거나 특정 날짜 범위에 대한 모델을 다시 정렬할 수 있습니다. 자세한 내용은 [모델 교육 및 점수](train-score.md#score)를 참조하십시오.


### 모델 삭제

모델을 삭제하려면

1. 왼쪽 레일에서 ![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]**&#x200B;을(를) 선택합니다.
1. 모델에 대해 ![자세히](/help/assets/icons/More.svg)를 선택하고 상황에 맞는 메뉴에서 **[!UICONTROL Delete]**&#x200B;을(를) 선택합니다. 또는 파란색 작업 표시줄에서 ![삭제](/help/assets/icons/Delete.svg) **[!UICONTROL Delete]**&#x200B;을(를) 선택합니다.
1. **[!UICONTROL Delete model]** 확인 대화 상자에서 **[!UICONTROL Delete]**&#x200B;을(를) 선택하여 모델을 삭제합니다. 취소할 **[!UICONTROL Cancel]**&#x200B;을(를) 선택하십시오.

여러 모델을 삭제하려면 다음을 수행합니다.

1. 여러 모델을 선택합니다.
1. 파란색 작업 표시줄에서 ![삭제](/help/assets/icons/Delete.svg) **[!UICONTROL Delete]**&#x200B;을(를) 선택하여 모델을 삭제합니다.
1. **[!UICONTROL Delete *x *모델]**확인 대화 상자에서&#x200B;**[!UICONTROL Delete]**을(를) 선택하여 모델을 삭제합니다. 취소할&#x200B;**[!UICONTROL Cancel]**을(를) 선택하십시오.

