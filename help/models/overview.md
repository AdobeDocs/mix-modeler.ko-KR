---
title: 모델
description: Adobe 믹스 모델러에서 모델을 구성하고 사용하는 방법에 대해 알아봅니다.
feature: Models
source-git-commit: ac17f5a9fcf036c8e689879578e4b745b789cea3
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 0%

---


# 모델

Adobe 믹스 모델러의 모델 기능을 통해 비즈니스 목표에 맞고 멀티터치 속성 및 마케팅 믹스 모델링 간 AI 기반 전환 학습이 지원되는 AI/ML 모델을 구성, 트레이닝 및 평가할 수 있습니다.

이 모델은 Adobe 믹스 모델러 애플리케이션 워크플로의 일부로 생성하는 조화로운 데이터를 기반으로 합니다.

모델을 생성하려면 다음을 선택할 때 사용할 수 있는 Mix Modeler 단계별 안내식 모델 구성 플로우를 사용합니다 **[!UICONTROL Guide me]**. 다음을 참조하십시오 [모델 만들기](create.md) 을 참조하십시오.

## 모델 관리

Adobe 믹스 모델러 인터페이스에서 현재 모델의 테이블을 보려면 다음을 수행합니다.

1. 선택 ![](../assets/icons/FileData.svg) **[!UICONTROL Models]** 왼쪽 레일에서.

1. 현재 모델의 표가 표시됩니다.

   테이블 열은 모델에 대한 세부 사항을 지정합니다.

   | 열 이름 | 세부 사항 |
   |---|---|
   | 이름 | 모델 이름 |
   | 설명 | 모델에 대한 설명 |
   | 전환 이벤트 | 모델에 대해 선택한 변환입니다. |
   | 데이터 세트 | 모델이 교육하고 평가하는 데 사용하는 데이터 세트입니다. 이것은 기본적으로 조화된 데이터 세트입니다. |
   | 실행 빈도 | 모델 교육의 실행 빈도입니다. |
   | 마지막 실행 | 모델의 마지막 교육 날짜 및 시간입니다. |
   | 마지막 실행 상태 | 모델 교육의 마지막 실행 상태입니다. <br/><span style="color:green">●</span> 성공<br/><span style="color:orange">●</span> 교육 문제<br/> <span style="color:orange">●</span> 교육 대기 중 <br/><span style="color:red">●</span> 실패 |

   {style="table-layout:auto"}

1. 목록에 표시되는 열을 변경하려면 다음을 선택합니다 ![열 설정](../assets/icons/ColumnSetting.svg) 열 켜기/끄기 ![확인](../assets/icons/Checkmark.svg) 또는 끔.

### 모델 삭제

모델을 삭제하려면

1. 삭제할 모델의 이름을 선택합니다.

1. 컨텍스트 메뉴에서 을(를) 선택합니다 **[!UICONTROL Delete]** 모델을 삭제합니다.

### 모델의 세부 정보 보기

모델의 세부 정보를 보려면 다음 작업을 수행하십시오.

1. 자세히 보려는 모델의 이름을 선택합니다.

1. 컨텍스트 메뉴에서 을(를) 선택합니다 **[!UICONTROL More]**. 오른쪽 창에 선택한 모델의 세부 정보가 표시됩니다.



### 모델 인사이트

>[!NOTE]
>
>이 선택은 성공적인 교육을 받은 모델(마지막 실행 상태가 성공인 모델)에서만 사용할 수 있습니다.
>

Adobe 믹스 모델러 인터페이스에서 모델의 통찰력을 보려면 다음을 수행합니다.

1. 선택 ![](../assets/icons/FileData.svg) **[!UICONTROL Models]** 왼쪽 레일에서.

1. 을(를) 가진 모델 이름 선택 **[!UICONTROL Last run status]** / <span style="color:green">●</span> **[!UICONTROL Success]** 다음에서 **[!UICONTROL Models]** 표

1. 컨텍스트 메뉴에서 을(를) 선택합니다 **[!UICONTROL Model Insights]**. (으)로 리디렉션됩니다. [모델 인사이트](insights.md).


