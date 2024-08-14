---
title: 감사 로그
description: Mix Modeler에서 감사 로그에 액세스하는 방법을 알아봅니다.
feature: Administration
exl-id: aa65aac5-bea4-43ff-b0d0-9e8a6a97d3ca
source-git-commit: 77a338ae568c854b99069b849a18661d413c501c
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 5%

---

# 감사 로그

시스템에서 수행되는 활동의 투명성과 가시성을 높이기 위해 Mix Modeler 워크플로우 내의 사용자 활동을 Experience Platform 감사 로그에 캡처하여 Mix Modeler 범주에 대한 사용자 중심의 변경 사항을 파악합니다. 이러한 로그는 문제 해결에 도움이 될 수 있는 감사 추적을 형성하며, 기업이 기업 데이터 관리 정책 및 규정 요구 사항을 효과적으로 준수하는 데 도움이 될 수 있습니다.

<!-- DO WE HAVE TO ADD THIS
If you are subject to the Health Insurance Portability and Accountability Act (HIPAA) and create, receive, maintain, or transmit permitted sensitive personal data through Mix Modeler, you are responsible for executing a BAA with Adobe and licensing Healthcare Shield.
-->

감사 로그는 누가 어떤 작업을 언제 수행했는지 알려 줍니다. 로그에 기록된 각 작업에는 작업 유형, 날짜 및 시간, 작업을 수행한 사용자의 이메일 ID 및 작업 유형과 관련된 추가 속성을 나타내는 메타데이터가 포함됩니다. Mix Modeler에서 사용자가 수행한 만들기, 업데이트 및 삭제 작업을 추적합니다.

감사 로그를 검사하려면 Mix Modeler 인터페이스에서 다음을 수행합니다.

1. **[!UICONTROL PRIVACY]**&#x200B;에서 ![작업 목록](/help/assets/icons/TaskList.svg) **[!UICONTROL Audits]**&#x200B;을(를) 선택하십시오.

1. **[!UICONTROL Audits]**&#x200B;에서 **[!UICONTROL Activity log]**&#x200B;을(를) 찾을 수 있습니다. 활동 로그에는 다음 Mix Modeler 범주, 작업 및 상태에 대한 항목이 표시됩니다.

   | 카테고리 | 작업 | 상태 |
   |---|---|---|
   | Mix Modeler 데이터 세트 규칙 | 만들기 | 허용 또는 거부 |
   | Mix Modeler 데이터 세트 규칙 | 업데이트 | 허용 또는 거부 |
   | Mix Modeler 데이터 세트 규칙 | 삭제 | 허용 또는 거부 |
   | Mix Modeler 필드 | 만들기 | 허용 또는 거부 |
   | Mix Modeler 필드 | 업데이트 | 허용 또는 거부 |
   | Mix Modeler 필드 | 삭제 | 허용 또는 거부 |
   | Mix Modeler 마케팅 접점 | 만들기 | 허용 또는 거부 |
   | Mix Modeler 마케팅 접점 | 업데이트 | 허용 또는 거부 |
   | Mix Modeler 마케팅 접점 | 삭제 | 허용 또는 거부 |
   | Mix Modeler 전환 | 만들기 | 허용 또는 거부 |
   | Mix Modeler 전환 | 업데이트 | 허용 또는 거부 |
   | Mix Modeler 전환 | 삭제 | 허용 또는 거부 |
   | Mix Modeler 모델 | 만들기 | 허용 또는 거부 |
   | Mix Modeler 모델 | 업데이트 | 허용 또는 거부 |
   | Mix Modeler 모델 | 삭제 | 허용 또는 거부 |
   | Mix Modeler 모델 | 재채점 | 허용 또는 거부 |
   | Mix Modeler 모델 | 복제 | 허용 또는 거부 |
   | Mix Modeler 모델 | 교육 / 재교육 | 허용 또는 거부 |
   | Mix Modeler 모델 | 메타데이터 다운로드/저장 | 허용 또는 거부 |
   | Mix Modeler 플랜 | 만들기 | 허용 또는 거부 |
   | Mix Modeler 플랜 | 업데이트 | 허용 또는 거부 |
   | Mix Modeler 플랜 | 관련 모델 변경 | 허용 또는 거부 |
   | Mix Modeler 데이터 조화 | 동기화 트리거 | 허용 또는 거부 |


1. 자세한 내용을 보려면 활동 로그에서 항목을 선택하여 패널을 엽니다.

   ![Mix Modeler 감사](/help/assets/mix-modeler-audit.png)

1. **[!UICONTROL Category]**, **[!UICONTROL Action]**, **[!UICONTROL Request ID]**, **[!UICONTROL User]**, **[!UICONTROL Status]** 또는 **[!UICONTROL Date]** 범위를 필터링하려면 ![필터](/help/assets/icons/Filter.svg)를 선택하십시오.

1. 활동 로그에 표시되는 열을 수정하려면 ![열](/help/assets/icons/ColumnSetting.svg)을 선택하고 **[!UICONTROL Customize table]** 대화 상자에서 표시할 열을 선택합니다. 선택 항목을 적용하려면 **[!UICONTROL Apply]**&#x200B;을(를) 선택하고 선택 항목을 취소하려면 **[!UICONTROL Cancel]**&#x200B;을(를) 선택합니다.

1. 감사 로그를 다운로드하려면 ![다운로드](/help/assets/icons/Download.svg) **[!UICONTROL Download log]**&#x200B;를 선택하십시오. **[!UICONTROL Download log]** 대화 상자에서 **[!UICONTROL CSV]** 또는 **[!UICONTROL JSON]**&#x200B;을(를) 형식으로 선택하고 **[!UICONTROL Download]**&#x200B;을(를) 선택합니다.

## 감사 로그 액세스

조직에서 이 기능을 활성화하면 활동이 발생할 때 감사 로그가 자동으로 수집됩니다. 수동으로 감사 로그 수집을 활성화할 필요가 없습니다.

감사 로그를 보고 내보내려면 감사 로그 액세스 액세스 제어 권한이 있어야 합니다. Mix Modeler 기능에 대한 개별 권한을 관리하는 방법을 알아보려면 [액세스 제어 설명서](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/home)를 참조하세요.
