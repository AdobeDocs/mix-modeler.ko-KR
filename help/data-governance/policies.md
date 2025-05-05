---
title: 정책
description: Mix Modeler에서 정책에 액세스하는 방법을 알아봅니다.
feature: Administration
exl-id: 4dba7c30-ad1e-4213-a2b0-afc55f2448a3
source-git-commit: 132dc18b84723358a7d65e2aaadd49cf1deb2dd8
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 1%

---

# 정책

워크플로우를 통해 모델을 만들고 모델의 구성을 제출하면 [정책 시행](https://experienceleague.adobe.com/ko/docs/experience-platform/data-governance/enforcement/overview#automatic-enforcement)에서 위반이 있는지 확인합니다. 정책 위반이 발생하면 하나 이상의 정책이 위반되었음을 나타내는 팝오버가 표시됩니다. 이 검사는 Experience Platform 내의 데이터 작업 및 마케팅 작업이 데이터 사용 정책을 준수하는지 확인하기 위한 것입니다.

기본적으로 Mix Modeler은 다음 레이블 및 마케팅 작업과 관련된 Adobe 정의 정책 위반을 확인합니다.

| 정책 이름 | 관련 레이블 | 연계된 마케팅 액션 |
|---|---|---|
| 사용 분석 및 사용자 기반 측정 제한 | C8 | Analytics |
| 데이터 과학 제한 | C9 | 데이터 과학 |
| 데이터 내보내기 제한 | C12 | 데이터 내보내기 |

위반 은 사용자가 직접 정의한 정책과 위 표에 나열된 모든 마케팅 작업을 포함하는 정책에 대해서도 확인됩니다.

데이터 세트 규칙을 작성하는 동안 정책을 위반하면 정책 위반에 대한 정보를 표시하는 팝오버가 표시됩니다.

For example:

- 연결된 레이블 [!UICONTROL C9] 및 연결된 마케팅 작업 [!UICONTROL Data Science]과(와) 함께 [!UICONTROL Restrict data science] 정책을 사용하도록 설정했습니다.
- 전환 데이터 스키마의 `totalCost` 필드에 [!UICONTROL C9] - [!UICONTROL No data science] 레이블을 적용했습니다.
- 특히 전환 데이터 스키마의 `totalCost` 필드를 이름이 `spend`이고 표시 이름이 `Spend`인 통합 필드에 매핑하는 데이터 집합 규칙을 설정하려고 합니다.

데이터 집합 규칙을 저장하려는 경우 위반된 정책 목록을 표시하는 **[!UICONTROL Data governance policy violation detected]** 팝업이 표시됩니다. 정책 이름을 선택하면 [!UICONTROL Violation summary]에 [!UICONTROL Entity], [!UICONTROL Type], [!UICONTROL Field] 및 [!UICONTROL Government labels]이(가) 적용된 [!UICONTROL Active data governance labels] 목록이 표시됩니다.

<!-- pending screenshot -->

조화된 데이터에 이미 사용된 스키마 필드에 데이터 사용 레이블을 적용하면 정책 위반에 대한 정보를 표시하는 팝오버가 표시됩니다.

For example:

- 특히 전환 데이터 스키마의 `totalCost` 필드를 이름이 `spend`이고 표시 이름이 `Spend`인 통합 필드에 매핑하는 데이터 집합 규칙을 설정했습니다.
- 통합 데이터를 한 번 이상 동기화했습니다([데이터 집합 규칙 - 데이터 동기화](/help/harmonize-data/dataset-rules.md#sync-data) 참조).
- 연결된 레이블 [!UICONTROL C9] 및 연결된 마케팅 작업 [!UICONTROL Data Science]과(와) 함께 [!UICONTROL Restrict data science] 정책을 사용하도록 설정합니다.
- 전환 데이터 스키마의 `totalCost` 필드에 [!UICONTROL C9] - [!UICONTROL No data science] 레이블을 적용하려고 합니다.

스키마 업데이트를 저장하려는 경우 위반된 정책 목록을 표시하는 **[!UICONTROL Data governance policy violation detected]** 팝업이 표시됩니다. [!UICONTROL Data Lineage] 목록에서 자세한 내용을 찾으려면 [!UICONTROL Violation summary]에서 정책 이름을 선택하십시오.

<!-- pending screenshot -->

## 위반이 팝오버를 감지했습니다.

검색된 데이터 거버넌스 정책 위반 팝오버는 위반에 대한 특정 정보를 제공합니다. 구성 워크플로와 직접 관련되지 않은 정책 설정 및 기타 측정값을 통해 이러한 위반을 해결할 수 있습니다. 예를 들어 특정 필드가 데이터 과학 용도로 사용할 수 있도록 레이블을 변경할 수 있습니다. 또는 모델이 데이터 사용 레이블이 있는 개체를 사용하지 않도록 모델 구성 자체를 수정할 수도 있습니다.

왼쪽 레일의 ![개인 정보](/help/assets/icons/Privacy.svg) **[!UICONTROL Policies]** 선택 항목에서는 Experience Platform의 [!UICONTROL Policies] 인터페이스에 액세스할 수 있으므로 정책, 레이블 및 마케팅 작업을 관리할 수 있습니다.

<!--
Currently,  Mix Modeler does not support all of the data governance functionality offered by Experience Platform. Field level access control is supported. See [Field level access control](../harmonize-data/dataset-rules.md#field-level-access-control)
-->

>[!MORELIKETHIS]
>
>[데이터 사용 정책 개요](https://experienceleague.adobe.com/ko/docs/experience-platform/data-governance/policies/overview)
>
>

