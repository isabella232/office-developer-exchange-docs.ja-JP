---
title: DeliveryReportEnabled (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2ab522bc-40ea-4e43-aa57-6d2562db35e9
description: DeliveryReportEnabled 要素は、DeliveryReportEnabled () フラグを表します。 DeliveryReportEnabled 要素は、内部使用のみを対象としています。 この要素はクライアントによって使用されません。
ms.openlocfilehash: 2a163b3e6ceaa169cc8f76f395b7d501419a31ed
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458475"
---
# <a name="deliveryreportenabled-soap"></a>DeliveryReportEnabled (SOAP)

**Deliveryreportenabled**要素は、 **deliveryreportenabled ()** フラグを表します。 **Deliveryreportenabled**要素は、内部使用のみを対象としています。 この要素はクライアントによって使用されません。 
  
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
|[組織のリレーションシップ設定 (SOAP)](organizationrelationshipsettings-soap.md) <br/> |1つの組織の組織上の関係のリストを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

DeliveryReportEnabled 要素のテキスト値が true の場合は、組織内のユーザーからの配信レポートを使用できることを示します。 値が false の場合は、配信レポートを抑制する必要があることを示します。
  
## <a name="remarks"></a>注釈

この要素を使用して、サーバーからの配信レポートを許可または抑制します。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目

- [Get組織の Relationshipsettings 操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

