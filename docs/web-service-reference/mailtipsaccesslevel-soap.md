---
title: MailTipsAccessLevel (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 730e349e-8250-4236-af53-cd9039c74d8f
description: MailTipsAccessLevel 要素は、MailTipsAccessLevel プロパティを表します。 MailTipsAccessLevel 要素は、内部使用のみ。 クライアントでは、この要素は使用されません。
ms.openlocfilehash: 35fb4aa56bbfa42ac4be196a379dc48aff5ec101
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832313"
---
# <a name="mailtipsaccesslevel-soap"></a>MailTipsAccessLevel (SOAP)

**MailTipsAccessLevel**要素は、 **MailTipsAccessLevel**プロパティを表します。 **MailTipsAccessLevel**要素は、内部使用のみ。 クライアントでは、この要素は使用されません。 
  
```XML
<MailTipsAccessLevel/>
```

 **string**
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
   
## <a name="remarks"></a>備考

この要素は、応答で返されるメール ヒントの詳細情報の最大量を指定します。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |スキーマの自動検出  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目



[GetOrganizationRelationshipSettings 操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

