---
title: DeliveryReportEnabled (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 2ab522bc-40ea-4e43-aa57-6d2562db35e9
description: DeliveryReportEnabled 要素は DeliveryReportEnabled() フラグを表します。 DeliveryReportEnabled 要素は内部でのみ使用できます。 この要素は、クライアントでは使用されません。
ms.openlocfilehash: 95fe62e25ca871171b398b17f3d03dff9235001b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510170"
---
# <a name="deliveryreportenabled-soap"></a>DeliveryReportEnabled (SOAP)

**DeliveryReportEnabled 要素** は **DeliveryReportEnabled() フラグを表** します。 **DeliveryReportEnabled 要素** は内部でのみ使用できます。 この要素は、クライアントでは使用されません。 
  
```XML
<DeliveryReportEnabled>true | false</DeliveryReportEnabled>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[OrganizationRelationshipSettings (SOAP)](organizationrelationshipsettings-soap.md) <br/> |1 つの組織の組織関係の一覧を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

DeliveryReportEnabled 要素のテキスト値が true の場合、組織内のユーザーからの配信レポートを使用できます。 false の値は、配信レポートを抑制する必要があります。
  
## <a name="remarks"></a>注釈

サーバーからの配信レポートを許可または抑制するには、この要素を使用します。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |正解  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetOrganizationRelationshipSettings 操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

