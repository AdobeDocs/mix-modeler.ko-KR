---
title: 데이터 거버넌스 개요
description: 수집된 경험 데이터를 제어할 수 있는 Experience Platform의 서비스 및 도구를 사용하는 방법을 알아봅니다. 따라서 비즈니스 관행, 법적 의무 및 개발 프로세스를 준수합니다.
feature: Administration
exl-id: 87407c29-e158-48bf-bde9-b3c16a16107e
source-git-commit: 0ee212a626986e4c721d0e58f2528d0ca1a9fdbf
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 1%

---

# 데이터 거버넌스 개요

Mix Modeler과 Experience Platform 간의 통합은 Mix Modeler에 Experience Platform의 고유한 데이터 거버넌스 기능을 활용할 수 있는 기능을 제공합니다. 이 설명서 섹션에서는 Mix Modeler에서 사용할 수 있는 데이터 거버넌스 기능의 세부 사항을 자세히 설명합니다.

Experience Platform 데이터 거버넌스는 Experience Platform을 통해 데이터가 취하는 여정 전반에 걸쳐 데이터를 제어하고 이해할 수 있는 기능을 제공합니다. 이 여정은 데이터 품질, 데이터 계보, 데이터 카탈로그 유지 등을 포함합니다.

Experience Platform에서 사용하는 데이터 세트에 생성된 데이터 사용 레이블 및 정책은 해당되는 경우 Mix Modeler에서 표시됩니다. 예를 들어 이러한 레이블은 조화된 데이터의 데이터 세트 규칙에 속하는 데이터 세트를 삭제할 때 사용자를 중지하거나 경고합니다. 또는 데이터 세트 규칙을 만들 때 사용자에 대해 제한된 스키마 필드를 숨깁니다.

데이터 거버넌스 통합을 통해 규정 준수를 보다 효율적으로 관리할 수 있습니다. 조직의 데이터 관리자는 사용을 제한하는 정책을 설정할 수 있습니다. 따라서 데이터 관리자에 의해 정의된 정책을 준수하는 데이터를 사용할 수 있습니다. 자세한 내용은 [레이블 및 정책](https://experienceleague.adobe.com/ko/docs/analytics-platform/using/cja-dataviews/data-governance)에 대한 설명서를 읽어 보십시오.

다음 데이터 거버넌스 기능을 사용할 수 있습니다.

| 기능 | 세부 사항 |
|---|---|
| 액세스 제어 | 역할 기반 액세스 제어 및 속성 기반(필드 수준) 액세스 제어가 지원됩니다. 자세한 내용은 [액세스 제어](access-controls.md)를 참조하십시오. |
| 감사 로그 | 사용자가 특정 Mix Modeler 카테고리를 만들거나, 업데이트하거나, 삭제하면 Experience Platform 감사 기능이 감사 로그에 활동을 기록합니다. 자세한 내용은 [감사 로그](audit-logs.md)를 참조하십시오. |
| 정책 | 통합 데이터 워크플로의 일부로 Experience Platform 정의 정책이 시행됩니다. 데이터 사용 레이블 위반은 사용자에게 보고되고 표시됩니다. 자세한 내용은 [정책](policies.md)을 참조하세요. |
| 암호화 | 모델의 입력 및 출력에 사용되는 모든 데이터 세트는 Experience Platform 지침을 따릅니다. Experience Platform 데이터 암호화는 사용되지 않는 데이터 및 전송 중인 데이터에 적용됩니다. |
| 데이터 위생 | 모델 입력 및 출력에 사용되는 모든 데이터 세트는 Experience Platform 지침을 따릅니다. Experience Platform은 다양한 유형의 데이터 만료 지원을 포함하여 고객 데이터 라이프사이클을 관리하는 도구 세트를 제공합니다. 통합 데이터의 일부로 사용되는 Experience Platform에서 소스 데이터 세트를 삭제하면 알림이 표시됩니다. 자세한 내용은 [데이터 집합 규칙](/help/harmonize-data/dataset-rules.md)을 참조하세요. |
| 고객 관리 키 | Privacy Security Shield 또는 Healthcare Shield 추가 기능과 함께 Mix Modeler에 라이선스를 부여한 경우 고객 관리 키 기능을 사용하여 Azure Key Vault를 활용하여 API를 통해 자신의 키를 가져올 수 있습니다. Mix Modeler의 모델 내에서 처리되는 데이터를 완벽하게 관리할 수 있습니다. |
