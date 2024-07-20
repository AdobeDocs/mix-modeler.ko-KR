---
title: 모델
description: Mix Modeler에서 모델을 구성하고 사용하는 방법에 대해 알아봅니다.
feature: Models
exl-id: c43d9bc9-4429-45c2-9247-bd24510a24be
source-git-commit: 9085363e951a4e306c64ad28f56e2c15b4a6029a
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---

# 모델

Mix Modeler의 모델 기능을 사용하면 비즈니스 목표에 맞고 멀티터치 속성 및 마케팅 믹스 모델링 간 AI 기반 전환 학습이 지원되는 AI/ML 모델을 구성, 트레이닝 및 평가할 수 있습니다.

이 모델은 Mix Modeler 애플리케이션 워크플로의 일부로 만드는 통합 데이터를 기반으로 합니다.

Mix Modeler의 모델은 마케터의 투자를 기반으로 지정된 결과를 측정 및/또는 예측하기 위해 사용되는 머신 러닝 모델입니다. 마케팅 접점 및 요약 수준 데이터를 입력으로 사용할 수 있습니다. Mix Modeler을 사용하면 매출, 판매 수량, 리드 등과 같은 다양한 변수, 차원 및 결과 세트를 기반으로 모델의 변형을 만들 수 있습니다.

모델은 다음을 필요로 합니다.

* 한 번의 전환,
* 요약 수준 데이터, 마케팅 접점 데이터(이벤트 데이터) 또는 둘 다로 구성된 하나 이상의 마케팅 접점(채널)
* 구성 가능한 전환 확인 기간
* 구성 가능한 교육 창.

모델은 다음을 선택적으로 포함할 수 있습니다.

* 외부 요인,
* 내부 요인,
* 채널별로 사전 변환을 색인화하는 소위 &#39;priors&#39;(해당 데이터를 관찰하기 전이나 전에 데이터의 지식 또는 불확실성을 나타내는 확률 분포)
* 지출 공유 - 마케팅 데이터가 희소할 때 상대 지출 공유를 프록시로 사용합니다.


## 모델 만들기

모델을 만들려면 **[!UICONTROL Open model canvas]**&#x200B;을(를) 선택할 때 사용할 수 있는 Mix Modeler 단계별 안내식 모델 구성 흐름을 사용하십시오. 자세한 내용은 [모델 만들기](create.md)를 참조하십시오.

## 모델 관리

Mix Modeler 인터페이스에서 현재 모델의 테이블을 보려면 다음을 수행합니다.

1. 왼쪽 레일에서 ![](/help/assets//icons/FileData.svg) **[!UICONTROL Models]**&#x200B;을(를) 선택합니다.

1. 현재 모델의 표가 표시됩니다.

   테이블 열은 모델에 대한 세부 사항을 지정합니다.

   | 열 이름 | 세부 사항 |
   |---|---|
   | 이름 | 모델 이름 |
   | 설명 | 모델에 대한 설명 |
   | 전환 이벤트 | 모델에 대해 선택한 변환입니다. |
   | 실행 빈도 | 모델 교육의 실행 빈도입니다. |
   | 마지막 실행 | 모델의 마지막 교육 날짜 및 시간입니다. |
   | 상태 | 모델 교육의 마지막 실행 상태입니다. <br/><span style="color:green">●</span> 성공<br/><span style="color:orange">●</span> 교육 문제<br/> <span style="color:orange">●</span> 교육 대기 중 <br/><span style="color:red">●</span> 실패 <br/><span style="color:gray">●</span> _(마지막 실행이 진행 중인 경우) |

   {style="table-layout:auto"}

1. 목록에 표시되는 열을 변경하려면 ![열 설정](/help/assets//icons/ColumnSetting.svg)을 선택하고 ![확인](/help/assets//icons/Checkmark.svg)을 설정하거나 해제합니다.


### 모델의 세부 정보 보기

모델의 세부 정보를 보려면 다음 작업을 수행하십시오.

1. 세부 정보가 포함된 팝업을 표시하려면 모델에 대한 ![정보](/help/assets//icons/Info.svg)을(를) 선택하십시오.



### 모델 인사이트

Mix Modeler 인터페이스에서 모델의 통찰력을 보려면 다음을 수행하십시오.

1. 왼쪽 레일에서 ![](/help/assets//icons/FileData.svg) **[!UICONTROL Models]**&#x200B;을(를) 선택합니다.

1. **[!UICONTROL Last run status]**&#x200B;이(가) <span style="color:green">●</span>인 모델 이름 선택 **[!UICONTROL Models]** 테이블의 **[!UICONTROL Success]**. 모델 인사이트는 정상적으로 훈련된 모델에서만 사용할 수 있습니다.

1. 컨텍스트 메뉴에서 **[!UICONTROL Model Insights]**&#x200B;을(를) 선택합니다. [모델 인사이트](insights.md)(으)로 리디렉션되었습니다.


### 재채점


Mix Modeler 인터페이스에서 모델을 다시 평가하려면 다음을 수행하십시오.

1. 왼쪽 레일에서 ![](/help/assets//icons/FileData.svg) **[!UICONTROL Models]**&#x200B;을(를) 선택합니다.

1. **[!UICONTROL Last run status]**&#x200B;이(가) <span style="color:green">●</span>인 모델 이름 선택 **[!UICONTROL Models]** 테이블의 **[!UICONTROL Success]**. 재점수는 성공적으로 훈련된 모델에서만 사용할 수 있습니다.

1. 컨텍스트 메뉴에서 **[!UICONTROL Re-score]**&#x200B;을(를) 선택합니다. 모델에 대한 업데이트된 상태를 표시하는 데 몇 분 정도 걸릴 수 있습니다.


### 모델 삭제

모델을 삭제하려면

1. 삭제할 모델의 이름을 선택합니다.

1. 컨텍스트 메뉴에서 **[!UICONTROL Delete]**&#x200B;을(를) 선택하여 모델을 삭제합니다.

   >[!WARNING]
   >
   >모델이 즉시 삭제됩니다.


