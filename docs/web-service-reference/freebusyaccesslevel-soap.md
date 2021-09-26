---
title: FreeBusyAccessLevel (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: a287b9c3-7fb6-4f2f-a8dc-15d4bc32394c
description: FreeBusyAccessLevel 要素は FreeBusyAccessLevel プロパティを表します。 FreeBusyAccessLevel 要素は内部でのみ使用できます。 この要素は、クライアントでは使用されません。
ms.openlocfilehash: 72ccc93f21596a866346b0fb7e959dfaa2199ddd
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546428"
---
# <a name="freebusyaccesslevel-soap"></a>FreeBusyAccessLevel (SOAP)

**FreeBusyAccessLevel** 要素は **FreeBusyAccessLevel プロパティを表** します。 **FreeBusyAccessLevel** 要素は内部でのみ使用できます。 この要素は、クライアントでは使用されません。 
  
```XML
<FreeBusyAccessLevel/>
```

 **string**
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
   
## <a name="remarks"></a>注釈

この要素は、応答で返される空き時間情報の最大量を指定し、外部で共有される空き時間情報データのレベルを示します。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|スキーマ名  <br/> |自動検出スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |正解  <br/> |
   
## <a name="see-also"></a>関連項目



[GetOrganizationRelationshipSettings 操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

