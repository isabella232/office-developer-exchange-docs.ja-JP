---
title: DeliveryReportEnabled (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2ab522bc-40ea-4e43-aa57-6d2562db35e9
description: DeliveryReportEnabled 要素は、DeliveryReportEnabled() フラグを表します。 DeliveryReportEnabled 要素は、内部使用のみ。 クライアントでは、この要素は使用されません。
ms.openlocfilehash: 089256a5f75ad92a4f11c5aaf3d175382eeee456
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760007"
---
# <a name="deliveryreportenabled-soap"></a>DeliveryReportEnabled (SOAP)

**DeliveryReportEnabled**要素は、 **DeliveryReportEnabled()** フラグを表します。 **DeliveryReportEnabled**要素は、内部使用のみ。 クライアントでは、この要素は使用されません。 
  
```XML
<DeliveryReportEnabled>true | false</DeliveryReportEnabled>
```

 **ブール型 (Boolean)**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[OrganizationRelationshipSettings (SOAP)](organizationrelationshipsettings-soap.md) <br/> |1 つの組織の組織との関係のリストを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

DeliveryReportEnabled 要素のテキスト値は、組織内のユーザーからの配信レポートを使用できることを示します。 False の値は、配信レポートを抑制する必要があることを示します。
  
## <a name="remarks"></a>備考

許可またはサーバーからの配信レポートを抑制するには、この要素を使用します。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |スキーマの自動検出  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetOrganizationRelationshipSettings 操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

