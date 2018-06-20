---
title: LegacyDN (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 9fb9529f-52c5-4907-a84b-935b78de16c3
description: LegacyDN 要素は、従来の識別名によって、ユーザーのメールボックスを識別します。
ms.openlocfilehash: f7ec1dea29a7d3ad6d470ef7812390d179fe1d2a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832243"
---
# <a name="legacydn-pox"></a>LegacyDN (POX)

**LegacyDN**要素は、従来の識別名によって、ユーザーのメールボックスを識別します。 
  
```xml
<LegacyDN/>
```

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[要求 (POX)](request-pox.md) <br/> |自動検出サービスへの要求が含まれています。  <br/> |
|[ユーザー (POX)](user-pox.md) <br/> |ユーザー固有の情報を提供します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、ユーザーの既存の電子メール アドレスを表します。
  
## <a name="remarks"></a>備考

[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)の要素は、自動検出要求の代替要素です。 Microsoft Exchange Server 2007 を実行しているコンピューター上にメールボックスが存在する場合に使用されます。 
  
## <a name="see-also"></a>関連項目

- [交換の POX の自動検出の XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

