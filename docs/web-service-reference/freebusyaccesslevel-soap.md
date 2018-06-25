---
title: FreeBusyAccessLevel (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: a287b9c3-7fb6-4f2f-a8dc-15d4bc32394c
description: FreeBusyAccessLevel 要素は、FreeBusyAccessLevel プロパティを表します。 FreeBusyAccessLevel 要素は、内部使用のみ。 クライアントでは、この要素は使用されません。
ms.openlocfilehash: c978608982a2795af1683b4b2121435a02149935
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760598"
---
# <a name="freebusyaccesslevel-soap"></a>FreeBusyAccessLevel (SOAP)

**FreeBusyAccessLevel**要素は、 **FreeBusyAccessLevel**プロパティを表します。 **FreeBusyAccessLevel**要素は、内部使用のみ。 クライアントでは、この要素は使用されません。 
  
```XML
<FreeBusyAccessLevel/>
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

この要素は、応答で返される空き時間情報の詳細情報の最大量を指定し、外部で共有されている空き時間情報データのレベルを示します。 
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |スキーマの自動検出  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目



[GetOrganizationRelationshipSettings 操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

