---
title: 관리
description: Mix Modeler 관리 방법을 알아봅니다.
feature: Administration
exl-id: 76d6d15d-a838-4ee2-9929-e55ea8946b80
source-git-commit: 4d84c93121fc476cc6610ad572bab161bbacfc23
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 2%

---

# 관리

사용 [Adobe Admin Console](https://helpx.adobe.com/enterprise/using/admin-console.html) Mix Modeler 제품 및 사용자를 관리합니다.

Mix Modeler이 제대로 작동하려면 올바른 권한을 설정해야 합니다.

Adobe Experience Cloud UI에서:

1. 선택 **[!UICONTROL Permissions]** 왼쪽 레일에서 아래 **[!UICONTROL ADMINISTRATION]**.

1. 선택 ![사용자](/help/assets/icons/User.svg) **[!UICONTROL Roles]** 왼쪽 패널에서 가져옵니다.

1. 기존 역할을 선택하거나 다음을 사용하여 역할을 만듭니다 **[!UICONTROL Create role]** (예: **Mix Modeler**). 기존 역할을 선택하는 경우 다음을 선택합니다 ![편집](/help/assets/icons/Edit.svg) **[!UICONTROL Edit]** 을 눌러 역할에 대한 권한을 편집합니다. 다음을 참조하십시오 [역할 관리](https://helpx.adobe.com/enterprise/using/admin-console.html) 추가 정보.

1. 역할에 대해 하나 이상의 샌드박스를 선택했는지 확인합니다.

1. 추가 **Adobe Mix Modeler** 리소스를 역할에 대한 리소스 목록으로 추가합니다.

1. 올바른 을(를) 선택하십시오. **[!UICONTROL Adobe Mix Modeler]** 구성 중인 역할에 대한 권한입니다. 다음 역할 중 하나 이상을 선택할 수 있습니다.

   - **[!UICONTROL View Adobe Mix Modeler Harmonized Data]**
   - **[!UICONTROL Manage Adobe Mix Modeler Harmonized Data]**
   - **[!UICONTROL View Adobe Mix Modeler Models Configuration]**
   - **[!UICONTROL Manage Adobe Mix Modeler Models Configuration]**
   - **[!UICONTROL View Adobe Mix Modeler Plans Configuration]**
   - **[!UICONTROL Manage Adobe Mix Modeler Plans Configuration]**

     ![MIX MODELER RBAC](/help/assets/mix-modeler-rbac.png)


1. 역할에 대한 추가 권한을 선택해야 합니다. 예를 들어 데이터 세트와 스키마를 보거나 관리하려면 다음을 선택합니다.

   - **[!UICONTROL Data Management]**: 관련 옵션을 선택합니다. **[!UICONTROL View Datasets]** 또는 **[!UICONTROL Manage Datasets]**.

   - **[!UICONTROL Data Modeling]**: 관련 옵션을 선택합니다. **[!UICONTROL Manage Schemas]** 또는 **[!UICONTROL View Schemas]**.

   <!--
    * **[!UICONTROL Data Governance]**: ensure you select **[!UICONTROL View User Activity Log]** and **[!UICONTROL View Data Usage Policies]**.
    -->

   <!--![Permissions](assets/permissions-including-privacy.png)-->

   선택 **[!UICONTROL Save]** 사용 권한을 저장합니다.

1. 위치 **[!UICONTROL Details]** 다음 범위 내 **[!UICONTROL Role]**&#x200B;을 클릭하고 적절한 을(를) 추가합니다. **[!UICONTROL Users]** 또는 **[!UICONTROL User groups]** 사용자에게 Mix Modeler에 대한 액세스 권한을 제공합니다.
