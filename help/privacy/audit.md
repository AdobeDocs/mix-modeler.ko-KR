---
title: 감사
description: Mix Modeler을 감사하는 방법을 알아봅니다.
feature: Administration
source-git-commit: e1ef6f2b54ae7c80cb115b417909b154b6153ce2
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 6%

---

# 감사

>[!AVAILABILITY]
>
>이 문서에 설명된 기능은 릴리스의 제한된 테스트 단계에 있으며 사용자 환경에서 아직 사용하지 못할 수 있습니다. 이 메모는 기능을 일반적으로 사용할 수 있을 때 제거됩니다. 최신 Mix Modeler 릴리스에 대한 자세한 내용은 [Mix Modeler 릴리스](/help/releases/latest.md).

Experience Platform의 감사 인터페이스 부분을 사용하고 Mix Modeler UI에 임베드되어 Mix Modeler에서 사용자가 수행하는 작업을 감사할 수 있습니다.

감사 로그를 검사하려면 Mix Modeler 인터페이스에서 다음을 수행합니다.

1. 선택 ![작업 목록](../assets/icons/TaskList.svg) **[!UICONTROL Audits]** 출처: **[!UICONTROL PRIVACY]**.

1. 위치 **[!UICONTROL Audits]** 다음을 찾을 수 있습니다. **[!UICONTROL Activity log]**. 활동 로그에는 다음 Mix Modeler 범주, 작업 및 상태에 대한 항목이 표시됩니다.

   | 카테고리 | 작업 | 상태 |
   |---|---|---|
   | Mix Modeler 데이터 세트 규칙 | 만들기 | 허용 또는 거부됨 |
   | Mix Modeler 데이터 세트 규칙 | 업데이트 | 허용 또는 거부됨 |
   | Mix Modeler 데이터 세트 규칙 | 삭제 | 허용 또는 거부됨 |
   | Mix Modeler 필드 | 만들기 | 허용 또는 거부됨 |
   | Mix Modeler 필드 | 업데이트 | 허용 또는 거부됨 |
   | Mix Modeler 필드 | 삭제 | 허용 또는 거부됨 |
   | Mix Modeler 마케팅 접점 | 만들기 | 허용 또는 거부됨 |
   | Mix Modeler 마케팅 접점 | 업데이트 | 허용 또는 거부됨 |
   | Mix Modeler 마케팅 접점 | 삭제 | 허용 또는 거부됨 |
   | Mix Modeler 전환 | 만들기 | 허용 또는 거부됨 |
   | Mix Modeler 전환 | 업데이트 | 허용 또는 거부됨 |
   | Mix Modeler 전환 | 삭제 | 허용 또는 거부됨 |
   | Mix Modeler 모델 | 만들기 | 허용 또는 거부됨 |
   | Mix Modeler 모델 | 업데이트 | 허용 또는 거부됨 |
   | Mix Modeler 모델 | 삭제 | 허용 또는 거부됨 |

1. 자세한 내용을 보려면 활동 로그에서 항목을 선택하여 패널을 엽니다.

   ![Mix Modeler 감사](../assets/mix-modeler-audit.png)

1. 필터링 대상 **[!UICONTROL Category]**, **[!UICONTROL Action]**, **[!UICONTROL Request ID]**, **[!UICONTROL User]**, **[!UICONTROL Status]** 또는 **[!UICONTROL Date]** 범위, 선택 ![필터](../assets/icons/Filter.svg).

1. 작업 로그에 표시되는 열을 수정하려면 다음을 선택합니다. ![열](../assets/icons/ColumnSetting.svg) 및 **[!UICONTROL Customize table]** 대화 상자에서 표시할 열을 선택합니다. 선택 **[!UICONTROL Apply]** 선택 항목을 적용하려면 **[!UICONTROL Cancel]** 선택 항목을 취소합니다.

1. 감사 로그를 다운로드하려면 다음을 선택합니다. ![다운로드](../assets/icons/Download.svg) **[!UICONTROL Download log]**. 다음에서 **[!UICONTROL Download log]** 대화 상자에서 다음 중 하나를 선택합니다. **[!UICONTROL CSV]** 또는 **[!UICONTROL JSON]** 을(를) 형식으로 설정하고 을(를) 선택합니다. **[!UICONTROL Download]**.

