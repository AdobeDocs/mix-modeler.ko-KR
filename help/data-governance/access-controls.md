---
title: 액세스 제어
description: Mix Modeler에서 액세스 제어를 구성하는 방법에 대해 알아봅니다.
feature: Administration
exl-id: c9ec97d9-b9a2-41f5-8626-1cf967d5d7fe
source-git-commit: 9a6c1f1c12ab29da80a1997cfd31ca07b38eaa22
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 1%

---

# 액세스 제어

Mix Modeler에 대한 액세스 제어는 [Adobe Admin Console](https://adminconsole.adobe.com/)의 Experience Platform 및 Experience Platform의 [권한](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/home#platform-permissions)을 통해 제공됩니다. 이 기능은 사용 권한 및 샌드박스를 사용자와 연결하는 Admin Console의 제품 프로필을 활용합니다.

액세스 제어에 대한 자세한 내용은 [액세스 제어 개요](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/home)를 참조하십시오.

## 역할 기반 액세스 제어

Experience Platform의 Mix Modeler 사용자 및 사용자 그룹에 대한 역할 기반 액세스 권한을 구성하는 방법에 대해서는 [관리](../main-guide/administration.md)를 참조하십시오.

## 속성 기반 액세스 제어

[특성 기반 액세스 제어](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/abac/overview)는 관리자가 특성을 기반으로 특정 개체 및/또는 기능에 대한 액세스를 제어할 수 있도록 해주는 Experience Platform 기능입니다. 속성은 스키마 필드 또는 세그먼트에 추가된 레이블과 같이 객체에 추가된 메타데이터일 수 있습니다. 관리자는 사용자 액세스 권한을 관리하기 위해 속성이 포함된 액세스 정책을 정의합니다.

이 기능을 사용하면 XDM(Experience Data Model) 스키마 필드에 조직 또는 데이터 사용 범위를 정의하는 레이블로 레이블을 지정할 수 있습니다. 동시에 관리자는 사용자 및 역할 관리 인터페이스를 사용하여 XDM 스키마 필드에 대한 액세스 정책을 정의할 수 있습니다. 또한 사용자 또는 사용자 그룹(내부, 외부 또는 서드파티 사용자)에 부여된 액세스를 더 잘 관리할 수 있습니다. 또한 속성 기반 액세스 제어를 통해 관리자는 특정 세그먼트에 대한 액세스를 관리할 수 있습니다.

속성 기반 액세스 제어를 통해 관리자는 모든 플랫폼 워크플로 및 리소스에서 중요한 개인 데이터(SPD)와 개인 식별 정보(PII) 모두에 대한 사용자의 액세스를 제어할 수 있습니다. 관리자는 특정 필드 및 해당 필드에 해당하는 데이터에만 액세스할 수 있는 사용자 역할을 정의할 수 있습니다.

조화된 데이터 세트에 대한 데이터 세트 규칙을 구성할 때 Experience Platform의 [특성 기반 액세스 제어](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/abac/overview)가 필드 수준에서 적용됩니다. 레이블이 스키마 필드에 첨부된 경우 필드는 제한됩니다. 그리고 해당 필드에 대한 액세스를 거부하는 활성 정책이 활성화됩니다. 그 결과는 다음과 같습니다.

* 데이터 세트 규칙을 만들 때 제한된 스키마 필드는 표시되지 않습니다.
* 제한된 하나 이상의 스키마 필드의 매핑을 보거나 편집할 수 없습니다. 이러한 제한된 필드가 포함된 데이터 세트 규칙을 편집하거나 볼 때 다음 화면이 표시됩니다.
  ![액션이 허용되지 않음](/help/assets/action-not-permitted.png)
