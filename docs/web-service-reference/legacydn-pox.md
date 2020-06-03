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
description: LegacyDN 要素は、ユーザーのメールボックスを従来の識別名で識別します。
ms.openlocfilehash: b9af4278a5421dc932573396c3563a64a78de41e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526383"
---
# <a name="legacydn-pox"></a>LegacyDN (POX)

**LegacyDN**要素は、ユーザーのメールボックスを従来の識別名で識別します。 
  
```xml
<LegacyDN/>
```

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[要求 (POX)](request-pox.md) <br/> |自動検出サービスへの要求を含みます。  <br/> |
|[ユーザー (POX)](user-pox.md) <br/> |ユーザー固有の情報を提供します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、ユーザーの従来の電子メールアドレスを表します。
  
## <a name="remarks"></a>注釈

[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)要素は、自動検出要求の代替要素です。 これは、Microsoft Exchange Server 2007 を実行しているコンピューター上にメールボックスが存在する場合に使用されます。 
  
## <a name="see-also"></a>関連項目

- [Exchange の POX 自動検出 XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

